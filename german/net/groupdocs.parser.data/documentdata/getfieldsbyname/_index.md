---
title: "GetFieldsByName"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Gibt die Sammlung von Felddaten zurück, bei denen der Name gleich fieldName ist."
type: docs
weight: 50
url: /de/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---

## DocumentData.GetFieldsByName method

Gibt die Sammlung von Felddaten zurück, bei denen der Name gleich *fieldName* ist.

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | String | Der Name des Feldes. |

### Rückgabewert

Eine Sammlung von [`FieldData`](../../fielddata)-Objekten; leere Sammlung, wenn keine Felddaten gefunden werden.

### Beispiele

Felder nach einem Feldnamen finden:

```csharp
// Alle Felder mit dem Namen "Address" abrufen
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // Über die Feldsammlung iterieren
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // Wenn es ein verwandtes Feld ist:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields.

### Siehe auch

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
