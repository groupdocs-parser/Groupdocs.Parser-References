---
title: "PageRenderInfo"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente les informations sur la façon dont une page est rendue."
type: docs
weight: 500
url: /fr/net/groupdocs.parser.options/pagerenderinfo/
---

## PageRenderInfo class

Représente les informations sur la façon dont une page est rendue.

```csharp
public sealed class PageRenderInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageRenderInfo](pagerenderinfo)(int, int, int) | Initialise une nouvelle instance de la classe [`PageRenderInfo`](../pagerenderinfo). |

## Propriétés

| Nom | Description |
| --- | --- |
| [ColumnCount](../../groupdocs.parser.options/pagerenderinfo/columncount) { get; } | Obtenez le nombre total de colonnes de tuiles. |
| [PageNumber](../../groupdocs.parser.options/pagerenderinfo/pagenumber) { get; } | Obtient le numéro de page. |
| [RowCount](../../groupdocs.parser.options/pagerenderinfo/rowcount) { get; } | Obtenez le nombre total de lignes de tuiles. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetColumn](../../groupdocs.parser.options/pagerenderinfo/getcolumn)(int) | Renvoie l'index de la colonne où la tuile avec *tileIndex* est placée. |
| [GetRow](../../groupdocs.parser.options/pagerenderinfo/getrow)(int) | Renvoie l'index de la ligne où la tuile avec *tileIndex* est placée. |

### Remarques

Certains documents (les feuilles de calcul, par exemple) ne peuvent pas être rendus en une seule image de page. Pour ces documents, une page est rendue sous forme d'ensemble de tuiles. Ces tuiles sont placées dans un tableau rectangulaire.

[`RowCount`](./rowcount) and [`ColumnCount`](./columncount) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
