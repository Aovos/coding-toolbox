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
|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Zeichensatz|`<meta charset="UTF-8">`|Sorgt dafür, dass Umlaute/ Sonderzeichen korrekt dargestellt werden|
|Viewport|`<meta name="viewport" content="width=device-width, initial-scale=1.0">`|Sorgt für richtige Skalierung auf Smartphones und Tablets|
|Titel|`<title>`|Titel der Seite → wird im Browser‑Tab angezeigt|
---

### `<body>`

##### Text-Überschrift
|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Kommentar|`<!-- [Text] -->`|Wird im Browser nicht angezeigt -> kann auch mehrzeilig als Kommentarblock genutzt werden (einfach --> später setzen).)|<!-- [Mein Text] -->|
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
|Zeilenumbruch|`...<br>`|Text geht über mehrere Zeilen (bleibt aber ein Absatz)|Zeile 1<br>Zeile 2<br>Zeile 3|
|Textfeld (statisch)|`<pre>...</pre>`|Ein statisches Textfeld -> Text wird genau so abgebildet|<pre>Statisches    Text f e l d</pre>|

##### Text-Formatierungen
|Code‑Element:|Code:|Beschreibung:|Beispiel:|
|-|-|-|-|
|Fett|`<b>...</b>`|Macht Text fett|<b>Text</b>|
|Kursiv|`<i>...</i>`|Macht Text kursiv|<i>Text</i>|
|Unterstrichen|`<u>...</u>`|Unterstreicht Text|<u>Text</u>|
|Durchgestrichen|`<s>...</s>`|Zeigt Text als „nicht mehr gültig“|<s>Text</s>|
|Kleinerer Schrift|`<small>...</small>`|Zeigt Text kleiner an|<small>Text</small>|
|Hochgestellt|`<sup>...</sup>`|	Hochgestellter Text|2<sup>3</sup>|
|Tiefgestellt|`<sub>...</sub>`|Tiefgestellter Text|H<sub>2</sub>O|
|Inline Code|`<code>...</code>`|Markiert kurze Codebegriffe im Fließtext|Das<code>hier</code>|

