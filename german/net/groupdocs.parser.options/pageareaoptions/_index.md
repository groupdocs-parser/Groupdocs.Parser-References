---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion von Seitenbereichen verwendet werden."
type: docs
weight: 460
url: /de/net/groupdocs.parser.options/pageareaoptions/
---

## PageAreaOptions class

Stellt die Optionen bereit, die für die Extraktion von Seitenbereichen verwendet werden.

```csharp
public class PageAreaOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageAreaOptions](pageareaoptions#constructor)() | Initialisiert eine neue Instanz der [`PageAreaOptions`](../pageareaoptions)-Klasse. |
| [PageAreaOptions](pageareaoptions#constructor_1)(Rectangle) | Initialisiert eine neue Instanz der [`PageAreaOptions`](../pageareaoptions)-Klasse. |
| [PageAreaOptions](pageareaoptions#constructor_2)(Rectangle, double) | Initialisiert eine neue Instanz der [`PageAreaOptions`](../pageareaoptions)-Klasse mit der Größe des ignorierten Randes. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Liest den rechteckigen Bereich, der Seitenbereiche enthält. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Liest die Größe des Randes, der beim Erfassen durch den rechteckigen Bereich ignoriert wird. Er wird als Bruchteil der Höhe eines Textelements gemessen. |

### Hinweise

Eine Instanz der [`PageAreaOptions`](../pageareaoptions)-Klasse wird als Parameter in den folgenden Methoden verwendet:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)

Siehe dort die Anwendungsbeispiele.

### Siehe auch

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
