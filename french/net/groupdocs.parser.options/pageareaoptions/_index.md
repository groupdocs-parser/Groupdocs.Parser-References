---
title: "PageAreaOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options utilisées pour l'extraction des zones de page."
type: docs
weight: 460
url: /fr/net/groupdocs.parser.options/pageareaoptions/
---

## PageAreaOptions class

Fournit les options utilisées pour l'extraction des zones de page.

```csharp
public class PageAreaOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageAreaOptions](pageareaoptions#constructor)() | Initialise une nouvelle instance de la classe [`PageAreaOptions`](../pageareaoptions). |
| [PageAreaOptions](pageareaoptions#constructor_1)(Rectangle) | Initialise une nouvelle instance de la classe [`PageAreaOptions`](../pageareaoptions). |
| [PageAreaOptions](pageareaoptions#constructor_2)(Rectangle, double) | Initialise une nouvelle instance de la classe [`PageAreaOptions`](../pageareaoptions) avec la taille de la bordure ignorée. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Obtient la zone rectangulaire qui contient les zones de page. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |

### Remarques

Une instance de la classe [`PageAreaOptions`](../pageareaoptions) est utilisée comme paramètre dans les méthodes suivantes:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)

Voir les exemples d'utilisation là-bas.

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
