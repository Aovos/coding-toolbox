[<- Zurück](../Grundaufbau.md)
# Externe Einbettungen

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Externe Inhalte einbetten|`<iframe src="URL" Optionen></iframe>`|Bindet externe Inhalte wie Webseiten, YouTube‑Videos, Karten oder Tools ein.|

### Iframe‑Attribute (Optionen)

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Breite setzen|`width="600"`|Legt die Breite des eingebetteten Inhalts fest (Pixel oder %)|
|Höhe setzen|`height="400"`|Legt die Höhe fest (Pixel oder %)|
|Rahmen deaktivieren|`frameborder="0"`|Entfernt den iframe‑Rahmen (wird oft genutzt)|
|Vollbild erlauben|`allowfullscreen`|Erlaubt, dass der externe Inhalt im Vollbild angezeigt werden kann|
|Sicherheits‑/Zugriffsrechte|`allow="..."`|Erlaubt Funktionen wie z.B. `autoplay`, `clipboard-write`, `encrypted-media` usw.|
|Ladeverhalten|`loading="lazy"`|Lädt das iframe erst, wenn es sichtbar wird (Performance‑Optimierung)|
