[<- Zurück](../Grundaufbau.md)

# Tabellen

### Grundaufbau
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
### Tabellen Beispiel

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
