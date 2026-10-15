---
title: "PageArea"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Liefert den Wert des Feldes."
type: docs
weight: 30
url: /de/net/groupdocs.parser.data/fielddata/pagearea/
---

## FieldData.PageArea property

Liefert den Wert des Feldes.

```csharp
public PageArea PageArea { get; }
```

### Property Value

Eine Instanz der [`PageArea`](../../pagearea)-Klasse, die den Wert des Feldes darstellt.

### Beispiele

Abhängig vom Feld kann die `PageArea`-Eigenschaft beliebige Unterklassen der [`PageArea`](../../pagearea)-Klasse enthalten. Zum Beispiel extrahiert die Methode [`ParseForm`](../../../groupdocs.parser/parser/parseform) nur Textfelder.

```csharp
// Hole die Felddaten
FieldData field = data[i];
// Prüfe, ob die Felddaten einen Text enthalten
if(field.PageArea is PageTextArea)
{
    // Gib den Feldtextwert aus
    Console.WriteLine(field.Text);
}
```

### Siehe auch

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
