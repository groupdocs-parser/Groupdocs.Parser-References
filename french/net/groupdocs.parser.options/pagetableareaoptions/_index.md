---
title: "PageTableAreaOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options qui sont utilisées pour l'extraction des zones de tableau de page."
type: docs
weight: 510
url: /fr/net/groupdocs.parser.options/pagetableareaoptions/
---

## PageTableAreaOptions class

Fournit les options qui sont utilisées pour l'extraction des zones de tableau de page.

```csharp
public sealed class PageTableAreaOptions : PageAreaOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageTableAreaOptions](pagetableareaoptions)(TemplateTableLayout) | Initialise une nouvelle instance de la classe [`PageAreaOptions`](../pageareaoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Obtient la zone rectangulaire qui contient les zones de page. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |
| [TableLayout](../../groupdocs.parser.options/pagetableareaoptions/tablelayout) { get; } | Obtient la mise en page du tableau qui définit le tableau sur une page. |

### Remarques

Une instance de la classe [`PageTableAreaOptions`](../pagetableareaoptions) est utilisée comme paramètre dans les méthodes [`GetTables`](../../groupdocs.parser/parser/gettables) et [`GetTables`](../../groupdocs.parser/parser/gettables). Voir les exemples d’utilisation là‑bas.

### Voir aussi

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
