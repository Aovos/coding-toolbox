# Übersicht:
### Basics
- [Grundaufbau](#grundaufbau)
- [Metadaten](#meta-daten)
- [Dateipfade](./Module/Dateipfade.md)
---
### Text
- [Text‑Überschriften](./Module/Text-Überschrift.md)
- [Text-Struktur](./Module/Text-Struktur.md)
- [Text-Formatierungen](./Module/Text-Formatierungen.md)
---
### Inhaltselemente
- [Links](./Module/Links.md)
- [Bilder](./Module/Bilder.md)
- [Video&Audio](./Module/Video&Audio.md)
- [Externe Einbettungen (Embeds)](#externe-einbettungen)
- [Tabellen](#tabellen)

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


### Grundgerüst erklärt

|Abschnitt:|Beschreibung:|
|-|-|
|`<!DOCTYPE html>`|Deklaration -> sagt dem Browser, dass das Dokument HTML5 ist|
|`<html lang="de">`|HTML‑Tag -> Webseitesprache: Deutsch (zusätzliche Info)|
|`<head>`|Metainformationen -> Generelle Einstellungen (Titel, Zeichensatz, usw.)|
|`<body>`|Inhaltsbereich -> Alles was dargestellt wird (z.B. Text, Bilder, Videos, Buttons, usw.|
---

### `<head>`

##### Meta-Daten

|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Zeichensatz|`<meta charset="UTF-8">`|Legt die Zeichencodierung fest (Umlaute, Sonderzeichen)|/|
|Viewport|`<meta name="viewport" content="width=device-width, initial-scale=1.0">`|Sorgt für korrekte Darstellung (Skalierung) auf mobilen Geräten|/|
|Titel|`<title>Meine Seite</title>`|Titel der Webseite (steht im Browser‑Tab)|Webseite XYZ|
|Beschreibung|`<meta name="description" content="">`|Kurzbeschreibung für Suchmaschinen (SEO)|"Die Webseite macht das und das und das|
|Autor|`<meta name="author" content="">`|Gibt den Autor/Ersteller der Seite an|[Name des Autors]|

---

### `<body>`

### Strukturelemente im `<body>`
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

---


---

#### Externe Einbettungen

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Externe Inhalte einbetten|`<iframe src="URL" Optionen></iframe>`|Bindet externe Inhalte wie Webseiten, YouTube‑Videos, Karten oder Tools ein.|

##### Iframe‑Attribute (Optionen)

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Breite setzen|`width="600"`|Legt die Breite des eingebetteten Inhalts fest (Pixel oder %)|
|Höhe setzen|`height="400"`|Legt die Höhe fest (Pixel oder %)|
|Rahmen deaktivieren|`frameborder="0"`|Entfernt den iframe‑Rahmen (wird oft genutzt)|
|Vollbild erlauben|`allowfullscreen`|Erlaubt, dass der externe Inhalt im Vollbild angezeigt werden kann|
|Sicherheits‑/Zugriffsrechte|`allow="..."`|Erlaubt Funktionen wie z.B. `autoplay`, `clipboard-write`, `encrypted-media` usw.|
|Ladeverhalten|`loading="lazy"`|Lädt das iframe erst, wenn es sichtbar wird (Performance‑Optimierung)|

---

#### Tabellen
```
<table>   = der Rahmen / die komplette Tabelle

  <caption> = Tabellen-Überschrift (Titel der gesamten Tabelle)

  <thead>   = Kopfzeile der Tabelle
    <tr>    = Kopfzeile besteht aus Zeilen
      <th>  = Titelzellen -> Spalten-Titel-Elemente

  <tbody>   = Tabelleninhalt unter dem Tabellenkopf
    <tr>    = Tabellenzeilen
      <td>  = normale Datenzellen

  <tfoot>   = Tabellenfuß (z. B. Zusammenfassung, Stand, Hinweise)
```
##### Tabellen Beispiel
<table>
  <caption>Benutzerübersicht</caption>

  <thead>
    <tr>
      <th>Name</th>
      <th>Alter</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>Anna</td>
      <td>24</td>
    </tr>
    <tr>
      <td>Markus</td>
      <td>31</td>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <td colspan="2">Stand: 2026</td>
    </tr>
  </tfoot>
</table>

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Tabelle erstellen|`<table> ... </table>`|Erstellt eine Tabelle → äußerer Rahmen|
|Tabellen‑Titel|`<caption> ... </caption>`|Überschrift der gesamten Tabelle (steht direkt unter `<table>`!)|
|Tabellenkopf|`<thead> ... </thead>`|Kopfzeile der Tabelle – enthält die Spaltenüberschriften|
|Tabellenzeile (Kopf)|`<tr> ... </tr>`|Zeile im Tabellenkopf|
|Titelzelle|`<th> ... </th>`|Kopfzelle → Spalten‑ bzw. Zeilenüberschrift|
|Tabellenkörper|`<tbody> ... </tbody>`|Hauptinhalt der Tabelle (unter dem Tabellenkopf)|
|Tabellenzeile (Inhalt)|`<tr> ... </tr>`|Eine Datenzeile im Tabellenkörper|
|Datenzelle|`<td> ... </td>`|Normale Tabellenzelle (Inhalt)|
|Tabellenfuß|`<tfoot> ... </tfoot>`|Fußbereich der Tabelle – z. B. Summen, Standangaben, Hinweise|
|Spalten verbinden|`colspan="X"`|Verbindet mehrere Spalten zu einer einzigen Zelle|
|Zeilen verbinden|`rowspan="X"`|Verbindet mehrere Zeilen zu einer einzigen Zelle|

