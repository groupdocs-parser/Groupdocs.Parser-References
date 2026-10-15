---
title: "HighlightOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options qui sont utilisées pour extraire un surlignage d'un bloc de texte autour du texte trouvé dans les scénarios de recherche."
type: docs
weight: 360
url: /fr/net/groupdocs.parser.options/highlightoptions/
---

## HighlightOptions class

Fournit les options utilisées pour extraire une mise en évidence (un bloc de texte autour du texte trouvé dans les scénarios de recherche).

```csharp
public sealed class HighlightOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)() | Initialise une nouvelle instance de la classe [`HighlightOptions`](../highlightoptions) qui est utilisée pour extraire un surlignage de longueur fixe. |
| [HighlightOptions](highlightoptions#constructor_1)(int) | Initialise une nouvelle instance de la classe [`HighlightOptions`](../highlightoptions) qui est utilisée pour extraire un surlignage de longueur fixe. |
| [HighlightOptions](highlightoptions#constructor_2)(int?, bool) | Initialise une nouvelle instance de la classe [`HighlightOptions`](../highlightoptions) qui est utilisée pour extraire un surlignage limité à une ligne. |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int) | Initialise une nouvelle instance de la classe [`HighlightOptions`](../highlightoptions) qui est utilisée pour extraire un surlignage avec un nombre de mots fixe. |
| [HighlightOptions](highlightoptions#constructor_4)(int?, int?, bool) | Initialise une nouvelle instance de la classe [`HighlightOptions`](../highlightoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; set; } | Obtient la valeur qui indique si l'extraction du surlignage est limitée par le début (ou la fin) d'une ligne de texte. |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; set; } | Obtient une longueur maximale de texte. |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; set; } | Obtient un nombre maximal de mots. |

### Remarques

Une instance de la classe [`HighlightOptions`](../highlightoptions) est utilisée comme paramètre dans la méthode [`GetHighlight`](../../groupdocs.parser/parser/gethighlight). Voir les exemples d’utilisation là‑bas.

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
