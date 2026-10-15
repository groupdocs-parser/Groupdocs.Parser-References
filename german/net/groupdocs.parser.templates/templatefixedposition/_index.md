---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt eine Position des Vorlagenfeldes bereit, die durch den rechteckigen Bereich definiert ist."
type: docs
weight: 90
url: /de/net/groupdocs.parser.templates/templatefixedposition/
---

## TemplateFixedPosition class

Stellt eine Position des Vorlagenfeldes bereit, die durch den rechteckigen Bereich definiert ist.

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | Initialisiert eine neue Instanz der [`TemplateFixedPosition`](../templatefixedposition)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | Gibt den rechteckigen Bereich zurück, der das Vorlagenfeld enthält. |

### Beispiele

Dies ist der einfachste Weg, die Feldposition zu definieren. Es erfordert, einen rechteckigen Bereich auf der Seite festzulegen, der den Feldwert begrenzt. Der gesamte Text, der (auch teilweise) in den rechteckigen Bereich fällt, wird als Wert extrahiert:

```csharp
// Erstelle ein festes Vorlagenfeld mit dem Namen "Address", das durch ein Rechteck an der Position (35, 160) und mit der Größe (110, 20) begrenzt wird
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### Siehe auch

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
