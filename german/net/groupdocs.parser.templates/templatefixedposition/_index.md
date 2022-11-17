---
title: TemplateFixedPosition
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Stellt eine Vorlagenfeldposition bereit die durch den rechteckigen Bereich definiert wird.
type: docs
weight: 630
url: /de/net/groupdocs.parser.templates/templatefixedposition/
---
## TemplateFixedPosition class

Stellt eine Vorlagenfeldposition bereit, die durch den rechteckigen Bereich definiert wird.

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | Initialisiert eine neue Instanz von[`TemplateFixedPosition`](../templatefixedposition) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | Ruft den rechteckigen Bereich ab, der das Vorlagenfeld enthält. |

### Beispiele

Dies ist die einfachste Art, die Feldposition zu definieren. Es muss ein rechteckiger Bereich auf der Seite festgelegt werden, der den Feldwert begrenzt. Der gesamte Text, der (auch teilweise) in dem rechteckigen Bereich enthalten ist, wird als Wert extrahiert:

```csharp
// Erstellen Sie ein festes Vorlagenfeld mit dem Namen "Adresse", das an der Position (35, 160) und mit der Größe (110, 20) durch ein Rechteck begrenzt wird.
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### Siehe auch

* class [TemplatePosition](../templateposition)
* namensraum [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* Montage [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->