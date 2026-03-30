[<- Zurück](./Grundaufbau.md)
# Formular

Formulare dienen zur Eingabe und Übermittlung von Benutzerdaten. Alle Felder wie Eingaben, Auswahlfelder und Buttons werden in einem `<form>`-Element zusammengefasst.





## Grundaufbau

```html
<form action="ziel.php" method="post">
  <!-- Formularelemente -->
</form>
```

|Code-Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Formular erstellen|`<form>`|Umschließt alle Eingabefelder und Buttons|`<form action="login.php" method="post">`|
|action|`action="ziel.php"`|Zieladresse/Datei, an die die Formulardaten gesendet werden|`action="/absenden.php"`|
|method|`method="post/get"`|Art der Datenübertragung (GET sichtbar, POST verborgen)|`method="post"`|

## Labels

Labels verbinden Text mit einem Eingabefeld (`for` → `id`).

|Code-Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Label|`<label for="id">`|Text, der mit einem Feld verknüpft ist|`<label for="email">E-Mail</label>`|
|Verknüpfung|`for="id"`|Zeigt auf das zugehörige Eingabefeld|`for="pw"`|

## Eingabefeld Text

|Typ|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Text|`<input type="text">`|Standard-Textfeld|Name, Adresse|
|E-Mail|`<input type="email">`|E-Mail-Adresse (mit Validierung)|info@example.com|
|Passwort|`<input type="password">`|Eingabe wird verdeckt dargestellt|******|
|Telefon|`<input type="tel">`|Telefonnummer|+49 123 4567|
|URL|`<input type="url">`|Webadresse|https://example.com|

## Eingabefeld Zahlen & Datum

|Typ|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Number|`<input type="number">`|Zahlenfeld, optional mit Begrenzung|min/max|
|Date|`<input type="date">`|Datumsauswahl|2026-03-30|
|Time|`<input type="time">`|Uhrzeitauswahl|14:30|
|Datetime|`<input type="datetime-local">`|Datum + Uhrzeit|2026-03-30T14:30|

# Kontrollfelder (Checkbox & Radio)

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

# Textarea

```html
<textarea rows="4" cols="40"></textarea>
```

|Code-Element|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Textarea|`<textarea>`|Mehrzeiliges Texteingabefeld|Kommentar, Nachricht|
|rows/cols|`rows="" cols=""`|Sichtbare Größe festlegen|`rows="5"`|

# Auswahllisten (Select)

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

# Buttons

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

# Gruppierung (fieldset & legend)

```html
<fieldset>
  <legend>Persönliche Daten</legend>
  <label for="v">Vorname</label>
  <input type="text" id="v">
</fieldset>
```

|Element|Code|Beschreibung|
|-|-|-|
|Fieldset|`<fieldset>`|Gruppiert Formularbereiche|
|Legend|`<legend>`|Titel der Gruppe|

# Wichtige Attribute

|Attribut|Code|Beschreibung|Beispiel|
|-|-|-|-|
|Pflichtfeld|`required`|Eingabe ist notwendig|`<input required>`|
|Platzhalter|`placeholder="Text"`|Hilfstext im Feld|`placeholder="Name eingeben"`|
|Vorgabewert|`value=""`|Vorbelegung|`value="Max"`|
|Min/Max|`min="" max=""`|Grenzwerte für Zahlen|`min="18"`|
|Schrittweite|`step=""`|Zahlenabstand|`step="0.5"`|
|Vorab ausgewählt|`checked`|Checkbox/Radio aktiv|`checked`|
|Nicht veränderbar|`readonly`|Wert sichtbar aber nicht editierbar|`readonly`|
|Deaktiviert|`disabled`|Feld nicht verwendbar|`disabled`|

# Barrierefreiheit

|Empfehlung|Beschreibung|
|-|-|
|Label immer verwenden|Jedes Eingabefeld braucht ein zugehöriges `<label>`|
|Eindeutige IDs|Jedes Feld muss eine einzigartige `id` haben|
|Gruppierung nutzen|Radios und thematische Bereiche → immer mit `<fieldset>` + `<legend>`|

---
