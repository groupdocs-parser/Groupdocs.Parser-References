---
title: GetFieldsByName
second_title: GroupDocs.Parser voor .NET API-referentie
description: Geeft de verzameling veldgegevens terug waarvan de naam gelijk is aanfieldName .
type: docs
weight: 50
url: /nl/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---
## DocumentData.GetFieldsByName method

Geeft de verzameling veldgegevens terug waarvan de naam gelijk is aan*fieldName* .

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldName | String | De naam van het veld. |

### Winstwaarde

Een verzameling van[`FieldData`](../../fielddata) voorwerpen; lege verzameling als er geen veldgegevens worden gevonden.

### Voorbeelden

Zoek velden op een veldnaam:

[`FieldData`](../../fielddata) klasse vertegenwoordigt veldgegevens. Afhankelijk van het veld[`PageArea`](../../fielddata/pagearea) property kan elke erfgenaam van bevatten[`PageArea`](../../pagearea) klas. Bijvoorbeeld,[`ParseForm`](../../../groupdocs.parser/parser/parseform) methode extraheert alleen tekstvelden.

```csharp
// Haal alle velden op met de naam "Adres".
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // Herhaal de verzameling velden
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // Als het een gerelateerd veld is:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

### Zie ook

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* naamruimte [GroupDocs.Parser.Data](../../documentdata)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->