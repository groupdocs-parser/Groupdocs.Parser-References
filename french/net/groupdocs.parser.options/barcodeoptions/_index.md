---
title: "BarcodeOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit les options utilisées pour l'extraction de codes-barres."
type: docs
weight: 200
url: /fr/net/groupdocs.parser.options/barcodeoptions/
---

## BarcodeOptions class

Fournit les options utilisées pour l'extraction de codes-barres.

```csharp
public sealed class BarcodeOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [BarcodeOptions](barcodeoptions#constructor)() | Initialise une nouvelle instance de la classe [`BarcodeOptions`](../barcodeoptions) avec les valeurs par défaut. |
| [BarcodeOptions](barcodeoptions#constructor_1)(Rectangle) | Initialise une nouvelle instance de la classe [`BarcodeOptions`](../barcodeoptions) avec la zone rectangulaire. |
| [BarcodeOptions](barcodeoptions#constructor_3)(QualityMode, QualityMode, params string[]) | Initialise une nouvelle instance de la classe [`BarcodeOptions`](../barcodeoptions) avec les paramètres de qualité et les types de codes. |
| [BarcodeOptions](barcodeoptions#constructor_2)(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) | Initialise une nouvelle instance de la classe [`BarcodeOptions`](../barcodeoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowIncorrectBarcodes](../../groupdocs.parser.options/barcodeoptions/allowincorrectbarcodes) { get; set; } | Obtient la valeur indiquant si les codes-barres incorrects sont autorisés. |
| [BarcodeQuality](../../groupdocs.parser.options/barcodeoptions/barcodequality) { get; set; } | Obtient la qualité d'un code-barres source. |
| [CodeTypes](../../groupdocs.parser.options/barcodeoptions/codetypes) { get; set; } | Obtient les types de codes-barres à lire. |
| [Dimension](../../groupdocs.parser.options/barcodeoptions/dimension) { get; set; } | Obtient la taille minimale de l'élément minimal du code-barres. |
| [ImageQuality](../../groupdocs.parser.options/barcodeoptions/imagequality) { get; set; } | Obtient la qualité d'une image source. |
| [PagePreviewOptions](../../groupdocs.parser.options/barcodeoptions/pagepreviewoptions) { get; set; } | Obtient ou définit les options d'aperçu des pages du document. |
| [Rectangle](../../groupdocs.parser.options/barcodeoptions/rectangle) { get; set; } | Obtient la zone rectangulaire qui contient les zones de page. |

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
