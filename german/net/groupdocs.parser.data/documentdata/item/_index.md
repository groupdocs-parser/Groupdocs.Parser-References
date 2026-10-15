---
title: "Item"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Gibt die Felddaten anhand eines Index zurück."
type: docs
weight: 20
url: /de/net/groupdocs.parser.data/documentdata/item/
---

## DocumentData indexer

Gibt die Felddaten anhand eines Index zurück.

```csharp
public FieldData this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| index | Der nullbasierte Index des Feldes. |

### Rückgabewert

Eine Instanz der Klasse [`FieldData`](../../fielddata).

### Beispiele

Iteration über alle Felder:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields:

```csharp
// Parser erstellen
using (Parser parser = new Parser(filePath))
{
    // Daten aus PDF-Formular extrahieren
    DocumentData data = parser.ParseForm();
    // Über extrahierte Felder iterieren
    for (int i = 0; i < data.Count; i++)
    {
        // Das extrahierte Feld abrufen
        FieldData field = data[i];
        // Feldnamen ausgeben
        Console.Write(field.Name + ": ");
        // Prüfen, ob der Feldwert ein Text ist, und ihn ausgeben
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Siehe auch

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
