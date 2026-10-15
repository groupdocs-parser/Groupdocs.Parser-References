---
title: "OcrOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options utilisées pour le connecteur OCR."
type: docs
weight: 450
url: /fr/net/groupdocs.parser.options/ocroptions/
---

## OcrOptions class

Fournit les options utilisées pour le connecteur OCR.

```csharp
public class OcrOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OcrOptions](ocroptions#constructor)() | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions) avec une zone rectangulaire. |
| [OcrOptions](ocroptions#constructor_5)(OcrEventHandler) | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions) avec l'objet [`OcrEventHandler`](../ocreventhandler). |
| [OcrOptions](ocroptions#constructor_6)(PagePreviewOptions) | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions) avec une zone rectangulaire. |
| [OcrOptions](ocroptions#constructor_1)(Rectangle) | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions) avec une zone rectangulaire. |
| [OcrOptions](ocroptions#constructor_2)(Rectangle, OcrEventHandler) | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions) avec une zone rectangulaire et l'objet [`OcrEventHandler`](../ocreventhandler). |
| [OcrOptions](ocroptions#constructor_3)(Rectangle, OcrEventHandler, PagePreviewOptions, bool) | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions). |
| [OcrOptions](ocroptions#constructor_4)(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) | Initialise une nouvelle instance de la classe [`OcrOptions`](../ocroptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Handler](../../groupdocs.parser.options/ocroptions/handler) { get; set; } | Obtient le gestionnaire d'événements pour capturer les événements OCR. |
| [Language](../../groupdocs.parser.options/ocroptions/language) { get; set; } | Obtient ou définit la langue utilisée pour l'OCR. Détermine l'alphabet utilisé pendant la reconnaissance. L'anglais est utilisé par défaut. |
| [PagePreviewOptions](../../groupdocs.parser.options/ocroptions/pagepreviewoptions) { get; set; } | Obtient les options d'aperçu de la page du document. |
| [Rectangle](../../groupdocs.parser.options/ocroptions/rectangle) { get; set; } | Obtient la zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte. |
| [UseSpellChecker](../../groupdocs.parser.options/ocroptions/usespellchecker) { get; set; } | Obtient la valeur indiquant si le correcteur orthographique est utilisé. |

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
