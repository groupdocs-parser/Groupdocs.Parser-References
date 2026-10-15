---
title: "PageTableArea"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Représente une zone de tableau de page utilisée pour représenter un tableau dans la fonctionnalité d'analyse par modèle."
type: docs
weight: 840
url: /fr/net/groupdocs.parser.data/pagetablearea/
---

## PageTableArea class

Représente une zone de tableau de page utilisée pour représenter un tableau dans la fonctionnalité d'analyse par modèle.

```csharp
public sealed class PageTableArea : PageArea
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Cells](../../groupdocs.parser.data/pagetablearea/cells) { get; } | Obtient la collection de cellules. |
| [ColumnCount](../../groupdocs.parser.data/pagetablearea/columncount) { get; } | Obtient le nombre total de colonnes du tableau. |
| [Item](../../groupdocs.parser.data/pagetablearea/item) { get; } | Obtient la cellule du tableau par les index de ligne et de colonne. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Obtient les informations de la page du document telles que l'index de page et la taille de page. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Obtient la zone rectangulaire. |
| [RowCount](../../groupdocs.parser.data/pagetablearea/rowcount) { get; } | Obtient le nombre total de lignes du tableau. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetColumnWidth](../../groupdocs.parser.data/pagetablearea/getcolumnwidth)(int) | Renvoie la largeur de la colonne. |
| [GetRowHeight](../../groupdocs.parser.data/pagetablearea/getrowheight)(int) | Renvoie la hauteur de la ligne. |

### Remarques

[`PageTableArea`](../pagetablearea) class is used to organize inheritors of [`PageArea`](../pagearea) class in table structure.

### Voir aussi

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
