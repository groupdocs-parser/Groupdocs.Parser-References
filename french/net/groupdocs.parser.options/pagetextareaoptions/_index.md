---
title: "PageTextAreaOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options qui sont utilisées pour l'extraction des zones de texte de page."
type: docs
weight: 520
url: /fr/net/groupdocs.parser.options/pagetextareaoptions/
---

## PageTextAreaOptions class

Fournit les options qui sont utilisées pour l'extraction des zones de texte de page.

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)() | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec l'option d'utilisation d'OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec l'option d'utilisation d'OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec l'expression régulière. Les autres options sont définies par défaut (voir les remarques pour plus de détails). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(bool, OcrOptions) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec la possibilité de définir des options OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_6)(string, Rectangle) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec l'expression régulière et la zone rectangulaire. Les autres options sont définies par défaut (voir les remarques pour plus de détails). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_7)(string, Rectangle, double) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec l'expression régulière, la zone rectangulaire et la taille de la bordure ignorée. Les autres options sont définies par défaut (voir les remarques pour plus de détails). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, bool, bool, bool, Rectangle) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_5)(string, bool, bool, bool, Rectangle, double) | Initialise une nouvelle instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) avec la taille de la bordure ignorée. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; set; } | Obtient l'expression régulière. |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; set; } | Obtient la valeur indiquant si le formatage du texte est ignoré. |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; set; } | Obtient la valeur indiquant si la casse du texte n'est pas ignorée. |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; set; } | Obtient les options supplémentaires pour la fonctionnalité OCR. |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Obtient la zone rectangulaire qui contient les zones de page. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Obtient la taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; set; } | Obtient la valeur indiquant si les segments sont unis. |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; set; } | Obtient la valeur indiquant si la fonctionnalité OCR est utilisée pour extraire les zones de texte. |

### Remarques

Une instance de la classe [`PageTextAreaOptions`](../pagetextareaoptions) est utilisée comme paramètre dans les méthodes [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) et [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas). Voir les exemples d'utilisation à cet endroit. **En savoir plus:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Voir aussi

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
