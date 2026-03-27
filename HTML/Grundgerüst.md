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

##### Struktur
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

