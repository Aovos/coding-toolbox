# Aufbauindex:
### Basics
- [Grundaufbau](#grundaufbau)
- [Metadaten](#meta-daten)
- [Strukturelemente_im_body](#strukturelemente_im_body)
- [Dateipfade](./Module/Dateipfade.md)
---
### Text
- [Text‑Überschriften](./Module/Text-Überschrift.md)
- [Text-Strukturen](./Module/Text-Strukturen.md)
- [Text-Formatierungen](./Module/Text-Formatierungen.md)
---
### Inhaltselemente
- [Links](./Module/Links.md)
- [Bilder](./Module/Bilder.md)
- [Video&Audio](./Module/Video&Audio.md)
- [Embeds](./Module/Embeds.md)
- [Tabellen](./Module/Tabellen.md)
- [Formulare](./Module/Formular.md)

# Grundaufbau

```html
<!DOCTYPE html>
<html lang="de">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport"
      content="width=device-width,
      initial-scale=1.0">
    <title>Meine Seite</title>
    <meta name="description" content="Kurze, präzise Beschreibung der Seite.">
    <meta name="author" content="Dein Name">
  </head>
  <body>
    <!-- Sichtbarer Inhalt -->
  </body>
</html>
```

|Abschnitt:|Beschreibung:|
|-|-|
|`<!DOCTYPE html>`|Deklaration -> sagt dem Browser, dass das Dokument HTML5 ist|
|`<html lang="de">`|HTML‑Tag -> Webseitesprache: Deutsch (zusätzliche Info)|
|`<head>`|Metainformationen -> Generelle Einstellungen (Titel, Zeichensatz, usw.)|
|`<body>`|Inhaltsbereich -> Alles was dargestellt wird (z.B. Text, Bilder, Videos, Buttons, usw.|

## head

### Meta-Daten

|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Zeichensatz|`<meta charset="UTF-8">`|Legt die Zeichencodierung fest (Umlaute, Sonderzeichen)|/|
|Viewport|`<meta name="viewport" content="width=device-width, initial-scale=1.0">`|Sorgt für korrekte Darstellung (Skalierung) auf mobilen Geräten|/|
|Titel|`<title>Meine Seite</title>`|Titel der Webseite (steht im Browser‑Tab)|Webseite XYZ|
|Beschreibung|`<meta name="description" content="">`|Kurzbeschreibung für Suchmaschinen (SEO)|"Die Webseite macht das und das und das|
|Autor|`<meta name="author" content="">`|Gibt den Autor/Ersteller der Seite an|[Name des Autors]|

## body
### Strukturelemente_im_body
|Code|Code‑Element|Beschreibung|
|-|-|-|
|`<header>`|Kopfbereich|Enthält oft Logo, Titel, Navigation oder Suchleiste|
|`<nav>`|Navigation|Bereich für Menülinks oder andere Navigationselemente|
|`<main>`|Hauptinhalt|Der wichtigste Inhaltsbereich der Seite — darf **nur einmal** vorkommen|
|`<section>`|Abschnitt|Thematischer Bereich, gruppiert logisch zusammengehörige Inhalte|
|`<article>`|Artikel|Eigenständige Inhalte wie Blogposts, News oder Produktbeschreibungen|
|`<aside>`|Nebeninhalt|Sidebar, Werbung, ergänzende Infos oder weiterführende Links|
|`<footer>`|Fußbereich|Enthält z. B. Copyright, Kontakt, Impressum, Links|
|`<div>`|Block‑Container|Strukturelement -> für Layout & Gruppierung von Bereichen|

