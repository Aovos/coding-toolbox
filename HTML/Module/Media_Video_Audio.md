[<- Zurück](../Grundaufbau.md)
# Media_Video_Audio

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Video einbinden|`<video src="video.mp4" Optionen></video>`|Bindet ein Video ein|
|Audio einbinden|`<audio src="audio.mp3" Optionen></audio>`|Bindet eine Audio‑Datei ein|

### Media‑Attribute (Optionen)

|Code‑Element:|Code:|Beschreibung:|
|-|-|-|
|Steuerelemente|`controls`|Zeigt die Wiedergabe‑Steuerung an (Play/Pause, Lautstärke, Zeitlinie)|
|Automatisch abspielen|`autoplay`|Startet Video/Audio automatisch (wird oft blockiert, benötigt meist `muted`)|
|Wiederholen|`loop`|Spielt Video/Audio automatisch von vorne ab|
|Stumm starten|`muted`|Startet ohne Ton (notwendig für Autoplay auf modernen Browsern)|
|Vorschaubild (nur Video)|`poster="bild.jpg"`|Zeigt ein Vorschaubild, bevor das Video startet|
