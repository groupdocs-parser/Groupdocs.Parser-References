---
title: "SearchOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options qui sont utilisées pour la recherche de texte."
type: docs
weight: 590
url: /fr/net/groupdocs.parser.options/searchoptions/
---

## SearchOptions class

Fournit les options qui sont utilisées pour la recherche de texte.

```csharp
public sealed class SearchOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions) avec les valeurs par défaut. Voir les remarques pour plus de détails. |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions) qui est utilisée pour rechercher sans extraction de surlignage. |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions) qui est utilisée pour rechercher par pages et sans extraction de surlignage. |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions) qui est utilisée pour rechercher avec les mêmes options de surlignage pour l'extraction du surlignage gauche et droit. |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions) qui est utilisée pour rechercher avec les options de surlignage pour l'extraction du surlignage gauche et droit. |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions). |
| [SearchOptions](searchoptions#constructor_6)(bool, bool, bool, int, HighlightOptions, HighlightOptions) | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions) avec la limite de pages. |

## Propriétés

| Nom | Description |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; set; } | Obtient les options pour le surlignage gauche. |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; set; } | Obtient la valeur indiquant si la casse du texte n'est pas ignorée. |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; set; } | Obtient la valeur indiquant si la recherche de texte est limitée à un mot entier. |
| [MaxPageIndex](../../groupdocs.parser.options/searchoptions/maxpageindex) { get; set; } | Obtient la valeur qui représente l'index maximal de la page à rechercher. |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; set; } | Obtient les options pour le surlignage droit. |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; set; } | Obtient la valeur indiquant si la recherche est effectuée par pages. |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; set; } | Obtient la valeur indiquant si une expression régulière est utilisée. |

### Remarques

Une instance de la classe [`SearchOptions`](../searchoptions) est utilisée comme paramètre dans la méthode [`Search`](../../groupdocs.parser/parser/search). Voir les exemples d'utilisation là-bas.

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
