---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Stellt Parameter für die Tabellenerkennungs‑Algorithmen bereit."
type: docs
weight: 180
url: /de/net/groupdocs.parser.templates/templatetableparameters/
---

## TemplateTableParameters class

Stellt Parameter für die Tabellenerkennungs‑Algorithmen bereit.

```csharp
public sealed class TemplateTableParameters
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Initialisiert eine neue Instanz der [`TemplateTableParameters`](../templatetableparameters)-Klasse. |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Initialisiert eine neue Instanz der [`TemplateTableParameters`](../templatetableparameters)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Liefert den Wert, der angibt, ob die Tabelle zusammengeführte Zellen hat. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Liefert die minimale Anzahl der Tabellenspalten. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Liefert die minimale Anzahl der Tabellenzeilen. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Liefert den minimalen Abstand zwischen den Tabellenspalten. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Ermittelt den rechteckigen Bereich, der die Tabelle enthält. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Ermittelt die Spaltentrennzeichen der Tabelle. |

### Hinweise

Es gibt zwei Algorithmen, um eine Tabelle zu erkennen:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

In einigen Fällen, wenn Algorithmen eine Tabelle nicht erkennen können oder dies ungenau tun, wird die [`TemplateTableLayout`](../templatetablelayout)-Klasse verwendet.

### Siehe auch

* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
