[<- Zurück](../Grundaufbau.md)
# Formulare
> Formulare dienen zur Eingabe und Übermittlung von Benutzerdaten. Alle Felder wie Eingaben, Auswahlfelder und Buttons werden in einem `<form>`-Element zusammengefasst
## Grundaufbau

```html
<form action="ziel.php" method="post">
  <!-- Formularelemente -->
  label
  input
  textarea
  select
  buttons
  ...
  ..
  .
</form>
```


|Code-Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Formular erstellen|`<form>`|Umschließt alle Eingabefelder und Buttons|`<form action="login.php" method="post">`|
|action|`action="ziel.php"`|Zieladresse/Datei, an die die Formulardaten gesendet werden|`action="/absenden.php"`|
|method|`method="post/get"`|Art der Datenübertragung (GET=sichtbar offen, POST=versteckt & vertraulich)|`method="post"`|

## Index:
- [Grundaufbau](#grundaufbau)
- [Beispiel](#beispiel)
- [Gruppierung](#gruppierung)
- [Barrierefreiheit](#barrierefreiheit)
- [Labels](#labels)
- [Eingabefeld Text](#eingabefeld-text)
- [Checkbox--Radio](#checkbox--radio)
- [Textarea](#textarea)
- [Auswahllisten](#auswahllisten)
- [Buttons](#buttons)
- [Atribute](#atribute)

## Beispiel
``` html
<form action="ziel.php" method="post" enctype="multipart/form-data">

  <!-- Persönliche Daten -->
  <fieldset>
    <legend>Persönliche Daten</legend>

    <!-- Vorname -->
    <label for="vorname">Vorname</label>
    <input type="text" id="vorname" name="vorname" placeholder="Max" required>

    <!-- Alter -->
    <label for="alter">Alter</label>
    <input type="number" id="alter" name="alter" min="1" max="120">

    <!-- Geburtsdatum -->
    <label for="geburt">Geburtsdatum</label>
    <input type="date" id="geburt" name="geburt">
  </fieldset>


  <!-- Login / Zugangsdaten -->
  <fieldset>
    <legend>Login & Sicherheit</legend>

    <!-- E-Mail -->
    <label for="email">E-Mail</label>
    <input type="email" id="email" name="email" autocomplete="email">

    <!-- Passwort -->
    <label for="passwort">Passwort</label>
    <input type="password" id="passwort" name="passwort" minlength="8" required>
  </fieldset>


  <!-- Geschlecht -->
  <fieldset>
    <legend>Geschlecht</legend>

    <!-- Auswahl Radio Buttons -->
    <label><input type="radio" name="geschlecht" value="m"> Männlich</label>
    <label><input type="radio" name="geschlecht" value="w"> Weiblich</label>
    <label><input type="radio" name="geschlecht" value="d"> Divers</label>
  </fieldset>


  <!-- Kontakt & Auswahl -->
  <fieldset>
    <legend>Kontakt & Auswahl</legend>

    <!-- Lieblingsfarbe -->
    <label for="farbe">Lieblingsfarbe</label>
    <select id="farbe" name="farbe">
      <option value="rot">Rot</option>
      <option value="blau">Blau</option>
      <option value="grün">Grün</option>
    </select>

    <!-- Land -->
    <label for="land">Land</label>
    <input list="laender" id="land" name="land">
    <datalist id="laender">
      <option value="Deutschland">
      <option value="Österreich">
      <option value="Schweiz">
    </datalist>
  </fieldset>


  <!-- Nachricht -->
  <fieldset>
    <legend>Nachricht</legend>

    <!-- Textbereich -->
    <label for="nachricht">Nachricht</label>
    <textarea id="nachricht" name="nachricht" rows="4" cols="40"></textarea>
  </fieldset>


  <!-- Einstellungen -->
  <fieldset>
    <legend>Einstellungen</legend>

    <!-- Lautstärke -->
    <label for="bereich">Lautstärke</label>
    <input type="range" id="bereich" name="bereich" min="0" max="100">

    <!-- Farbwähler -->
    <label for="farbe_picker">Farbwahl</label>
    <input type="color" id="farbe_picker" name="farbe_picker" value="#ff0000">
  </fieldset>


  <!-- Datei-Upload -->
  <fieldset>
    <legend>Dateiupload</legend>

    <!-- Datei -->
    <label for="datei">Datei hochladen</label>
    <input type="file" id="datei" name="datei">
  </fieldset>


  <!-- AGB -->
  <label><input type="checkbox" name="agb" required> AGB akzeptieren</label>

  <!-- Buttons -->
  <button type="submit">Absenden</button>
  <button type="reset">Zurücksetzen</button>

</form>
```

## Gruppierung
```html
  <fieldset>
    <legend>Benennung/Überschrift des fieldsets</legend>
  </fieldset>
```

|Element|Code|Beschreibung|
|-|-|-|
|Fieldset|`<fieldset>`|Gruppiert Formularbereiche|
|Legend|`<legend>`|Titel der Gruppe|

## Barrierefreiheit

|Empfehlung|Beschreibung|
|-|-|
|Label immer verwenden|Jedes Eingabefeld braucht ein zugehöriges `<label>`|
|Eindeutige IDs|Jedes Feld muss eine einzigartige `id` haben|
|Gruppierung nutzen|Radios und thematische Bereiche → immer mit `<fieldset>` + `<legend>`|


## Labels
```html
<label for="id-name">Displayname</label>
<input type="text" id="id-name" name="übertragungsvariable" value="vordefinierterWert">
```

|Code-Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Label (Beschriftung)| `<label for="id">`| Sichtbarer Text für Benutzer & Screenreader. Beschriftet das Eingabefeld.| `<label for="email">E‑Mail</label>`|
|Verknüpfung Label → Input| `for="id"`| Verbindet Label mit Input über die gleiche `id`. Klick auf Label fokussiert das Feld.| `for="pw"`|
|Art der Eingabe (Input-Typ)|`type="text"`|Bestimmt die Art des Eingabefeldes (Text, Zahl, Passwort, E‑Mail, Datum …)|`type="email"`|
|ID des Eingabefeldes| `id="feld-id"`| Identifiziert das Eingabefeld im HTML. Wichtig für Label, CSS und JavaScript - Nicht relevant für Server‑Übertragung.|`id="email"`|
|Server‑Variablenname| `name="Server-Variable"`|Wichtigstes Formular‑Attribut. Unter diesem Namen wird der Wert(Value) an den Server übertragen.| `name="email"`|
|Value‑Holder (Optional)| `value="..."`| Startwert oder aktueller Wert des Feldes. Wird vom Benutzer überschrieben und beim Absenden zusammen mit `name` übertragen.|`value="info@test.de"`|

## Eingabefeld Text

|Typ|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Text|`<input type="text">`|Standard-Textfeld|Name, Adresse|
|E-Mail|`<input type="email">`|E-Mail-Adresse (mit Validierung)|info@example.com|
|Passwort|`<input type="password">`|Eingabe wird verdeckt dargestellt|******|
|Telefon|`<input type="tel">`|Telefonnummer|+49 123 4567|
|URL|`<input type="url">`|Webadresse|https://example.com|
|Number|`<input type="number">`|Zahlenfeld, optional mit Begrenzung|min/max|
|Date|`<input type="date">`|Datumsauswahl|2026-03-30|
|Time|`<input type="time">`|Uhrzeitauswahl|14:30|
|Datetime|`<input type="datetime-local">`|Datum + Uhrzeit|2026-03-30T14:30|

## Checkbox--Radio

```html
<input type="checkbox" id="agb">
<label for="agb">AGB akzeptieren</label>

<input type="radio" name="farbe" value="rot"> Rot
<input type="radio" name="farbe" value="blau"> Blau
```

|Typ|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Checkbox|`<input type="checkbox">`|Mehrfachauswahl möglich|AGB akzeptieren|
|Radio|`<input type="radio" name="x">`|Nur eine Auswahl bei gleichem `name`|Farbe wählen|

## Textarea

```html
<textarea rows="4" cols="40"></textarea>
```

|Code-Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Textarea|`<textarea>`|Mehrzeiliges Texteingabefeld|Kommentar, Nachricht|
|rows/cols|`rows="" cols=""`|Sichtbare Größe festlegen|`rows="5"`|

## Auswahllisten

```html
<select>
  <option>Rot</option>
  <option>Blau</option>
</select>
```

|Typ|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Select|`<select>`|Auswahlmenü|Farbauswahl|
|Option|`<option>`|Eintrag in Auswahl|Rot, Blau|
|Mehrfachauswahl|`<select multiple>`|Erlaubt mehrere ausgewählte Optionen|STRG+Klick|

## Buttons

```html
<button>Absenden</button>
<input type="submit" value="Senden">
<input type="reset" value="Zurücksetzen">
```

|Typ|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Button|`<button>`|Vielseitiger Button (mit Text oder HTML)|Absenden|
|Submit|`<input type="submit">`|Sendet Formular ab|Senden|
|Reset|`<input type="reset">`|Setzt alle Felder zurück|Zurücksetzen|

## Attribute


|Attribut|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Pflichtfeld|`required`|Eingabe ist notwendig|`<input required>`|
|Platzhalter|`placeholder="Text"`|Hilfstext im Feld|`placeholder="Name eingeben"`|
|Vorgabewert|`value=""`|Vorbelegung|`value="Max"`|
|||||
|Maximale Zeichen|`maxlength="Zahl"`|Begrenzt die maximale Zeichenanzahl|`maxlength="20"`|
|Minimale Zeichen|`minlength="Zahl"`|Eingabe muss mindestens X Zeichen haben|`minlength="3"`|
|Musterprüfung|`pattern="Regex"`|Validierung über regulären Ausdruck|`pattern="[A-Za-z]{3,}"`|
|||||
|Min/Max|`min="" max=""`|Grenzwerte für Zahlen|`min="18"`|
|Schrittweite|`step=""`|Zahlenabstand|`step="0.5"`|
|||||
|Mehrfachauswahl|`multiple`|Erlaubt mehrere Werte (file/select)|`<input type="file" multiple>`|
|Erlaubte Dateiarten|`accept="MimeTypes"`|Beschränkt erlaubte Dateitypen beim Upload|`accept="image/png"`|
|||||
|Vorab ausgewählt|`checked`|Checkbox/Radio aktiv|`checked`|
|Nicht veränderbar|`readonly`|Wert sichtbar aber nicht editierbar|`readonly`|
|Deaktiviert|`disabled`|Feld nicht verwendbar|`disabled`|
|||||
|Autocomplete|`autocomplete="off"`|Steuert Browser-Autovervollständigung|`autocomplete="email"`|
|Autofokus|`autofocus`|Feld wird automatisch fokussiert|`<input autofocus>`|
|Tooltip|`title="Text"`|Hinweis erscheint beim Hover|`title="Nur Buchstaben erlaubt"`|
|||||
|Zugehöriges Formular|`form="id"`|Ordnet Feld einem anderen Formular zu|`<input form="loginform">`|


