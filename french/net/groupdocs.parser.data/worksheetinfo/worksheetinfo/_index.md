---
title: "WorksheetInfo"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Initialise une nouvelle instance de la classe WorksheetInfogroupdocs.parser.data/worksheetinfo."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---

## WorksheetInfo constructor

Initialise une nouvelle instance de la classe [`WorksheetInfo`](../../worksheetinfo).

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L’indice basé sur zéro de la feuille de calcul. |
| nom | Chaîne | Une valeur de chaîne qui représente le nom de la feuille de calcul. |
| range | WorksheetRange | Une instance de la classe [`WorksheetRange`](../../worksheetrange) qui représente la taille de la feuille de calcul. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Un indice de la feuille de calcul ne peut pas être négatif. |
| ArgumentNullException | La taille de la feuille de calcul ne peut pas être `null`. |

### Voir aussi

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
