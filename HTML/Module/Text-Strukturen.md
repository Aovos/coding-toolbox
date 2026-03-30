[<- Zurück](../Grundaufbau.md)
# Text-Strukturen
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
