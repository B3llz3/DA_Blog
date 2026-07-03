# Travel Blog

Statisches Frontend-Projekt der Developer Akademie. Die Website bildet einen mehrseitigen Reiseblog mit Startseite, vier Artikelseiten und Impressum ab. Der Fokus liegt auf HTML- und CSS-Layout, responsiven Komponenten und einer einheitlichen visuellen Gestaltung ohne Build-Prozess oder Framework.

## Überblick

Die Startseite kombiniert eine Hero-Section, einen Highlights-Slider, einen FAQ-Bereich und ein Kontaktformular. Von dort aus gelangt man auf vier eigenständige Artikelseiten zu verschiedenen Reisezielen:

- `index.html`: Landingpage
- `article1.html`: Strände der Welt
- `article2.html`: Kopenhagen in 3 Tagen
- `article3.html`: Pattaya Pulse
- `article4.html`: Mt. Fuji
- `impressum.html`: rechtliche Angaben

## Features

- Statische Multi-Page-Website ohne JavaScript-Build-Setup
- Gemeinsame Navigation und Footer-Komponenten über mehrere Seiten
- Responsive Layouts mit separaten CSS-Dateien pro Seite
- CSS-basierter Slider auf der Startseite
- FAQ-Bereich mit `details`/`summary`
- Kontaktformular als UI-Komponente
- Externe Video-Einbettungen auf Artikelseiten

## Tech-Stack

- HTML5
- CSS3
- Lokale Assets für Icons, Bilder und Fonts
- Keine externen Frameworks
- Kein Package-Manager, kein Bundler, kein Backend

## Projektstruktur

```text
DA_Blog/
|-- index.html
|-- article1.html
|-- article2.html
|-- article3.html
|-- article4.html
|-- impressum.html
|-- css/
|   |-- index.css
|   |-- article1.css
|   |-- article2.css
|   |-- article3.css
|   |-- article4.css
|   |-- components.css
|   |-- layout.css
|   |-- variables.css
|   |-- font.css
|   `-- impressum.css
`-- assets/
    |-- fonts/
    |-- icons/
    `-- images/
```

## Lokale Nutzung

Da das Projekt rein statisch ist, gibt es keinen Installationsschritt.

1. Repository klonen oder lokal öffnen.
2. `index.html` direkt im Browser starten
3. Optional einen lokalen Server verwenden, z. B. mit VS Code Live Server oder:

```bash
python -m http.server 5500
```

Danach ist die Seite unter `http://localhost:5500` erreichbar.

## Styling-Konzept

- `variables.css` enthält zentrale CSS-Variablen.
- `layout.css` und `components.css` enthalten gemeinsame Layout- und UI-Bausteine.
- `font.css` bindet die verwendeten Schriften ein.
- Die Dateien `index.css` sowie `article1.css` bis `article4.css` enthalten seitenbezogene Styles.

## Inhaltlicher Aufbau

- `index.html` ist die Landingpage mit Navigation, Hero, Highlights, FAQ, Kontaktformular, Footer und Sticky-Footbar.
- Die Artikelseiten nutzen ein gemeinsames Grundlayout mit Intro, Autorensektion und individuellem Content.
- Bilder, Icons und Autorenfotos liegen unter `assets/`.

## Aktueller Stand / bekannte Einschränkungen

- Das Kontaktformular besitzt aktuell keine Formularverarbeitung.
- Der Link `Cookie Preferences` ist derzeit ein Platzhalter.
- Die Bildstruktur von Artikel 2 verwendet den Ordnernamen `assets/images/articel2/`.

## Team

Laut Impressum und Seiteninhalten wurde das Projekt von folgenden Personen erstellt:

- Alexander Jahn
- Daniel Gust
- Oliver Rittinghaus
- Steffen Schmidt

## Lizenz

Im Repository ist keine eigene Projektlizenz hinterlegt. Die Datei `LICENSE.txt` bezieht sich nicht offensichtlich auf den Inhalt dieser Website. Falls das Projekt veröffentlicht oder weiterverwendet werden soll, sollte eine eindeutige Lizenz ergänzt werden.
