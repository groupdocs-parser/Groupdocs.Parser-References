---
title: "TryParse"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Konvertiert die Zeichenkettenrepräsentation von Kanten in das entsprechende Klassenobjekt. Ein Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist."
type: docs
weight: 90
url: /de/net/groupdocs.parser.templates/templatelinkedpositionedges/tryparse/
---

## TemplateLinkedPositionEdges.TryParse method

Konvertiert die Zeichenkettenrepräsentation von Kanten in das entsprechende Klassenobjekt. Ein Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist.

```csharp
public static bool TryParse(string s, out TemplateLinkedPositionEdges edges)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | String | Eine Zeichenkette, die Kanten zum Konvertieren enthält. |
| edges | TemplateLinkedPositionEdges& | Wenn die Methode zurückkehrt, enthält sie die Instanz der Klasse [`TemplateLinkedPositionEdges`](../../templatelinkedpositionedges), die dem im Parameter *s* angegebenen Wert entspricht, wenn die Konvertierung erfolgreich war; andernfalls `null`. |

### Rückgabewert

`true`, wenn *s* erfolgreich konvertiert wird; andernfalls `false`.

### Siehe auch

* class [TemplateLinkedPositionEdges](../../templatelinkedpositionedges)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
