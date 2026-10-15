---
title: "WorksheetInfo"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Klasse WorksheetInfogroupdocs.parser.data/worksheetinfo."
type: docs
weight: 10
url: /de/net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---

## WorksheetInfo constructor

Initialisiert eine neue Instanz der Klasse [`WorksheetInfo`](../../worksheetinfo).

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | Int32 | Der nullbasierte Index des Arbeitsblatts. |
| name | String | Ein Zeichenkettenwert, der den Namen des Arbeitsblatts darstellt. |
| range | WorksheetRange | Eine Instanz der Klasse [`WorksheetRange`](../../worksheetrange), die die Größe des Arbeitsblatts darstellt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | Ein Index des Arbeitsblatts darf nicht negativ sein. |
| ArgumentNullException | Die Größe des Arbeitsblatts darf nicht `null` sein. |

### Siehe auch

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
