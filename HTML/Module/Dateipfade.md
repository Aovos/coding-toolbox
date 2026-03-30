[<- Zurück](../Grundaufbau.md)
# Dateipfade
`Alle eingebundenen Dateien (Bilder, Videos, Audio, CSS, JS, interne Links, Downloads …) verwenden dasselbe Pfadsystem.`

|Code‑Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Aktueller Ordner|`./`|Verweist auf den aktuellen Ordner (kann weggelassen werden)|`bild.jpg`|
|Eine Ebene höher|`../datei.txt`|Greift auf eine Datei im übergeordneten Ordner zu|`../datei.txt`|
|Zwei Ebenen höher|`../../datei.pdf`|Greift auf eine Datei zwei Ordner höher zu|`../../datei.pdf`|
|Drei Ebenen höher|`../../../datei.mp4`|Greift auf eine Datei drei Ordner höher zu|`../../../datei.mp4`|
|Datei im aktuellen Ordner|`bild.jpg`|Lädt eine Datei aus dem selben Ordner|`bild.jpg`|
|Datei im Unterordner|`unterordner/datei.png`|Greift auf Datei im Unterordner zu|`unterordner/datei.png`|
|Absolute URL|`https://example.com/...`|Externer Pfad zu Bild/Video/Datei|`https://example.com/logo.png`|

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
