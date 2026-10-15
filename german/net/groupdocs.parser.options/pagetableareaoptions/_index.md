---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion von Tabellenbereichen auf Seiten verwendet werden."
type: docs
weight: 510
url: /de/net/groupdocs.parser.options/pagetableareaoptions/
---

## PageTableAreaOptions class

Stellt die Optionen bereit, die für die Extraktion von Tabellenbereichen auf Seiten verwendet werden.

```csharp
public sealed class PageTableAreaOptions : PageAreaOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageTableAreaOptions](pagetableareaoptions)(TemplateTableLayout) | Initialisiert eine neue Instanz der [`PageAreaOptions`](../pageareaoptions)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Liest den rechteckigen Bereich, der Seitenbereiche enthält. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Liest die Größe des Randes, der beim Erfassen durch den rechteckigen Bereich ignoriert wird. Er wird als Bruchteil der Höhe eines Textelements gemessen. |
| [TableLayout](../../groupdocs.parser.options/pagetableareaoptions/tablelayout) { get; } | Ruft das Tabellenlayout ab, das die Tabelle auf einer Seite definiert. |

### Hinweise

Eine Instanz der Klasse [`PageTableAreaOptions`](../pagetableareaoptions) wird als Parameter in den Methoden [`GetTables`](../../groupdocs.parser/parser/gettables) und [`GetTables`](../../groupdocs.parser/parser/gettables) verwendet. Siehe dort die Anwendungsbeispiele.

### Siehe auch

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
