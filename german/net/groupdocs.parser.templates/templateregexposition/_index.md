---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt eine Vorlagenfeld‑Position bereit, die den regulären Ausdruck verwendet."
type: docs
weight: 150
url: /de/net/groupdocs.parser.templates/templateregexposition/
---

## TemplateRegexPosition class

Stellt eine Vorlagenfeld‑Position bereit, die den regulären Ausdruck verwendet.

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | Initialisiert eine neue Instanz der [`TemplateRegexPosition`](../templateregexposition)-Klasse. |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | Initialisiert eine neue Instanz der [`TemplateRegexPosition`](../templateregexposition)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | Ermittelt den regulären Ausdruck. |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | Ermittelt den Wert, der angibt, ob die Groß-/Kleinschreibung des Textes nicht ignoriert wird. |

### Beispiele

Das folgende Beispiel zeigt die Situation, wenn das Dokument "Invoice Number INV-12345" enthält, dann kann das Vorlagenfeld wie folgt definiert werden:

```csharp
// Erstelle ein Regex-Vorlagenfeld mit dem Namen "InvoiceNumber"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

In diesem Fall wird als Wert die gesamte Zeichenkette extrahiert. Um nur einen Teil der Zeichenkette zu extrahieren, wird die reguläre Ausdrucksgruppe "value" verwendet:

```csharp
// Erstelle ein Regex-Vorlagenfeld mit dem Namen "InvoiceNumber" und der Gruppe "value"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

In diesem Fall wird die Zeichenkette "INV-3337" als Wert extrahiert.

### Siehe auch

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
