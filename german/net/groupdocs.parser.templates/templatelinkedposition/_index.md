---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt eine Vorlagenfeld‑Position bereit, die das verknüpfte Feld verwendet."
type: docs
weight: 110
url: /de/net/groupdocs.parser.templates/templatelinkedposition/
---

## TemplateLinkedPosition class

Stellt eine Vorlagenfeld‑Position bereit, die das verknüpfte Feld verwendet.

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | Initialisiert eine neue Instanz der [`TemplateLinkedPosition`](../templatelinkedposition)-Klasse. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | Initialisiert eine neue Instanz der [`TemplateLinkedPosition`](../templatelinkedposition)-Klasse mit einem in GROSSBUCHSTABEN geschriebenen verknüpften Feldnamen. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_2)(string, Size, TemplateLinkedPositionEdges, bool, bool) | Initialisiert eine neue Instanz der [`TemplateLinkedPosition`](../templatelinkedposition)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | Gibt den Wert zurück, der angibt, ob [`SearchArea`](./searcharea) anhand der Größe des verknüpften Feldes skaliert wird. |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | Gibt die Kanten des verknüpften Feldes zurück, in dem ein Feld gesucht wird. |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | Gibt den Namen des verknüpften Feldes zurück. |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | Gibt die Größe des Bereichs zurück, in dem ein Feld gesucht wird. |

### Beispiele

Das folgende Beispiel zeigt den Code für den Fall, dass bekannt ist, dass das Feld mit einer Rechnungsnummer rechts vom String "Invoice number" platziert ist; der folgende Code wird verwendet:

```csharp
// Erstelle ein Regex‑Vorlagenfeld, um den Text "Invoice Number" zu finden
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// Erstelle ein zugehöriges Vorlagenfeld, das mit dem Feld "Invoice" verknüpft ist, und extrahiere den Wert rechts davon
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### Siehe auch

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
