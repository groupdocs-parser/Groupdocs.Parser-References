---
title: "TextOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options qui sont utilisées pour l'extraction de texte."
type: docs
weight: 610
url: /fr/net/groupdocs.parser.options/textoptions/
---

## TextOptions class

Fournit les options qui sont utilisées pour l'extraction de texte.

```csharp
public sealed class TextOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TextOptions](textoptions#constructor)() | Initialise une nouvelle instance de la classe [`TextOptions`](../textoptions). |
| [TextOptions](textoptions#constructor_1)(bool) | Initialise une nouvelle instance de la classe [`TextOptions`](../textoptions). |
| [TextOptions](textoptions#constructor_2)(bool, bool) | Initialise une nouvelle instance de la classe [`TextOptions`](../textoptions) avec l'option d'utilisation de l'OCR. |
| [TextOptions](textoptions#constructor_3)(bool, bool, OcrOptions) | Initialise une nouvelle instance de la classe [`TextOptions`](../textoptions) avec la possibilité de définir les options OCR. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IncludeAnnotations](../../groupdocs.parser.options/textoptions/includeannotations) { get; set; } | Obtient la valeur indiquant si les annotations sont incluses. La valeur par défaut est `false`. |
| [OcrOptions](../../groupdocs.parser.options/textoptions/ocroptions) { get; set; } | Obtient les options supplémentaires pour la fonctionnalité OCR. |
| [UseOcr](../../groupdocs.parser.options/textoptions/useocr) { get; set; } | Obtient la valeur qui indique si le OCR Connector est utilisé pour extraire un texte. |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; set; } | Obtient la valeur qui indique si le mode brut est utilisé. |

### Remarques

Une instance de la classe [`TextOptions`](../textoptions) est utilisée comme paramètre dans les méthodes [`GetText`](../../groupdocs.parser/parser/gettext) et [`GetText`](../../groupdocs.parser/parser/gettext). Voir les exemples d’utilisation là‑bas.

Il est utilisé pour spécifier le mode brut d’extraction de texte. Un texte dans ce mode est extrait de manière non précise mais plus rapidement que dans le mode standard. Si le mode brut ne prend pas en charge le format du document, ce paramètre est alors ignoré et le mode standard est utilisé.

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
