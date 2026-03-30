Übersicht:
- [Grundgerüst](#grundgerüst)
- [Metadaten](#meta-daten)
- [Text-Überschrift](#text-überschrift)
- [Text-Struktur](#text-struktur)
- [Text-Formatierungen](#text-formatierungen)
- [Dateipfade in HTML](#dateipfade-in-html)
- [Links](#links)
- [Bilder](#bilder)
- [Media (Video & Audio)](#media-video-&-audio)
- [Externe Einbettungen (Embeds)](#externe-einbettungen)
- [Tabellen](#tabellen)

# Grundgerüst

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


##### Text-Überschrift
|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Kommentar|`<!-- [Text] -->`|Wird im Browser nicht angezeigt -> kann auch mehrzeilig als Kommentarblock genutzt werden (einfach --> später setzen).)|<! -- Kommentar -->|
|Hauptüberschrift|`<h1>...</h1>`|Haupttitel einer Seite verwendet -> (Darf nur einmal verwendet werden!)|<h1>Hauptüberschrift</h1>|
|Kapitel-Überschrift|`<h2>...</h2>`|Strukturiert Inhalte unterhalb der H1|<h2>Kapitel</h2>|
|Unterkapitel 3|`<h3>...</h3>`|Strukturiert Inhalte unterhalb der H2 |<h3>Unterkapitel</h3>|
|Unterkapitel 4|`<h4>...</h4>`|Unterkapitel in der Ebene 4 (seltener)|<h4>Unterkapitel</h4>|
|Unterkapitel 5|`<h5>...</h5>`|Unterkapitel in der Ebene 5 (seltener)|<h5>Unterkapitel</h5>|
|Unterkapitel 6|`<h6>...</h6>`|Unterkapitel in der Ebene 6 (seltener)|<h6>Unterkapitel</h6>|

##### Text-Struktur
|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Absatz|`<p>...</p>`|Einfacher Text Abssatz -> (z.B. als würde man in Word einfach drauf los tippen)|<p>Mein Text</p>|
|Code-Block|`<pre><code>...</code></pre>`|Code-Block -> mehrzeiliger Inhaltsbereich, der sich vom restlichen Text absetzt.|<pre><code>Code-Block</code></pre>|
|Textfeld (statisch)|`<pre>...</pre>`|Ein statisches Textfeld -> Text wird genau so abgebildet|<pre>Statisches    Text f e l d</pre>|
|Zeilenumbruch|`...<br>`|Text geht über mehrere Zeilen (bleibt aber ein Absatz)|Zeile 1<br>Zeile 2<br>Zeile 3|
|Trennlinie|`<hr>`|Fügt eine horizontale Trennlinie hinzu|<hr>|
|Unordered List|`<ul><li>Eintrag</li></ul>`|Aufzählung - ohne Reihenfolge (Bulletlist)|<ul><li>Milch</li><li>Brot</li><li>Waschmittel</li></ul>|
|Ordered List|`<ol><li>...</li><li>...</li></ol>`|Geordnete Liste - Aufzählung|<ol><li>Schritt</li><li>Schritt</li><li>Schritt</li></ol>|
|Definition List|`<dl><dt>...</dt><dd>...</dd></dl>`|dt=Definition Term      dd=Definitions Beschreibung (beide müssen angegeben werden|<dl><dt>RAID ausgeschrieben?</dt><dd>Redundant Array of Independent Disks</dd></dl>|

##### Text-Formatierungen
|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Semantisch Wichtig|`<strong>...</strong>`|Kennzeichnet wichtige/bedeutungsvolle Informationen|<strong>Backup‑Geschwindigkeit:</strong> Bis zu 40% schneller mit der neuen Engine.|
|Semantisch betont|`<em>...</em>`|Markiert Wörter, die beim Lesen betont werden sollen|Ich habe <em>wirklich</em> alles versucht.|
|Fett|`<b>...</b>`|Macht Text fett|<b>Text</b>|
|Kursiv|`<i>...</i>`|Macht Text kursiv|<i>Text</i>|
|Unterstrichen|`<u>...</u>`|Unterstreicht Text|<u>Text</u>|
|Durchgestrichen|`<s>...</s>`|Zeigt Text als „nicht mehr gültig“|<s>Text</s>|
|Kleinerer Schrift|`<small>...</small>`|Zeigt Text kleiner an|<small>Text</small>|
|Hochgestellt|`<sup>...</sup>`|	Hochgestellter Text|2<sup>3</sup>|
|Tiefgestellt|`<sub>...</sub>`|Tiefgestellter Text|H<sub>2</sub>O|
|Inline Code|`<code>...</code>`|Markiert kurze Codebegriffe im Fließtext|Das<code>hier</code>|
|Inline‑Markierung|`<span>...</span>`|Markiert kleine Textbereiche, die individuell mit CSS gestaltet werden sollen|Dies ist ein <span>markiertes Wort</span>|

---

#### Dateipfade in HTML
`Alle eingebundenen Dateien (Bilder, Videos, Audio, CSS, JS, interne Links, Downloads …) verwenden dasselbe Pfadsystem.`
```
./                        → aktueller Ordner (kann weggelassen werden)
../datei.txt              → eine Ebene höher
../../datei.pdf           → zwei Ebenen höher
../../../datei.mp4        → drei Ebenen höher
usw.

Beispiele:
bild.jpg                  → Datei im aktuellen Ordner
https://example.com/...   → absolute URL (externes Bild/Video/Datei)
unterordner/datei.png     → Datei im Unterordner (Ordnernamen immer ausschreiben!)
```

---

#### Links

|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Standard‑Link|`<a href="URL">…</a>`|Erstellt einen klickbaren Link zu einer anderen Webseite|<a href="https://example.com">Beispiel</a>|
|Interner Link|`<a href="seite.html">…</a>`|Verlinkt auf eine Datei innerhalb derselben Webseite (Datei muss existieren!)|<a href="kontakt.html">Kontakt</a>|
|Mail‑Link|`<a href="mailto:adresse@example.com">…</a>`|Öffnet das Standard‑Mailprogramm mit der Adresse|<a href="mailto:info@example.com">E‑Mail senden</a>|
|Telefon‑Link|`<a href="tel:0123456789">…</a>`|Auf Smartphones anrufbar|<a href="tel:0123456789">Jetzt anrufen</a>|

###### Link‑Attribute (Optionen)
|Attribut|Code|Beschreibung|
|-|-|-|
|Neuer Tab|`target="_blank"`|Öffnet den Link in einem neuen Browser‑Tab|
|Tooltip|`title="Text"`|Zeigt beim Hover einen Hinweistext (Tooltip) an|
|Download|`download`|Erzwingt das Herunterladen der verlinkten Datei|
|Download mit Dateiname|`download="Dateiname.ext"`|Legt einen eigenen Dateinamen für den Download fest|

---

#### Bilder

|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Bild einfügen|`<img src="bild.jpg" alt="Beschreibung">`|Zeigt ein Bild an. `src` = Pfad zur Datei, `alt` = Beschreibung für Screenreader & SEO|<img src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg" alt="GitHub">|
|Bildbreite setzen|`<img src="bild.jpg" width="300">`|Legt die sichtbare Breite des Bildes fest (in Pixeln oder %) |<img src="https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg" width="300">|
|Bildhöhe setzen|`<img src="bild.jpg" height="200">`|Legt die sichtbare Höhe des Bildes fest|<img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Debian-OpenLogo.svg" alt="Debian Logo">|
|Bildgrößen frei skalieren|`<img src="bild.jpg" width="300" height="200">`|Breite & Höhe gleichzeitig setzen (Achtung: verzerrt das Bild!)|<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f9/Archlinux-logo-standard-version.svg/1920px-Archlinux-logo-standard-version.svg.png" width="300" height="200" alt="Arch Linux Logo">|

---

#### Media Video & Audio


|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Video einbinden|`<video src="video.mp4" Optionen></video>`|Bindet ein Video ein|
|Audio einbinden|`<audio src="audio.mp3" Optionen></audio>`|Bindet eine Audio‑Datei ein|

##### Media‑Attribute (Optionen)

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Steuerelemente|`controls`|Zeigt die Wiedergabe‑Steuerung an (Play/Pause, Lautstärke, Zeitlinie)|
|Automatisch abspielen|`autoplay`|Startet Video/Audio automatisch (wird oft blockiert, benötigt meist `muted`)|
|Wiederholen|`loop`|Spielt Video/Audio automatisch von vorne ab|
|Stumm starten|`muted`|Startet ohne Ton (notwendig für Autoplay auf modernen Browsern)|
|Vorschaubild (nur Video)|`poster="bild.jpg"`|Zeigt ein Vorschaubild, bevor das Video startet|

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

