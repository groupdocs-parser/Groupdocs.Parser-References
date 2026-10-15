---
title: "TemplateTableParameters"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit des paramètres pour les algorithmes de détection de tableau."
type: docs
weight: 180
url: /fr/net/groupdocs.parser.templates/templatetableparameters/
---

## TemplateTableParameters class

Fournit des paramètres pour les algorithmes de détection de tableau.

```csharp
public sealed class TemplateTableParameters
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Initialise une nouvelle instance de la classe [`TemplateTableParameters`](../templatetableparameters). |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Initialise une nouvelle instance de la classe [`TemplateTableParameters`](../templatetableparameters). |

## Propriétés

| Nom | Description |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Obtient la valeur qui indique si le tableau possède des cellules fusionnées. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Obtient le nombre minimum de colonnes du tableau. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Obtient le nombre minimum de lignes du tableau. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Obtient l'espacement minimum entre les colonnes du tableau. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Obtient la zone rectangulaire qui contient le tableau. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Obtient les séparateurs des colonnes du tableau. |

### Remarques

Il existe deux algorithmes pour détecter un tableau :

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

Dans certains cas, lorsque les algorithmes ne peuvent pas détecter un tableau ou le font de manière imprécise, la classe [`TemplateTableLayout`](../templatetablelayout) est utilisée.

### Voir aussi

* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
