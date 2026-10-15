---
title: "PreviewOptions"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçu."
type: docs
weight: 550
url: /fr/net/groupdocs.parser.options/previewoptions/
---

## PreviewOptions class

Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçu.

```csharp
public class PreviewOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Initialise une nouvelle instance de la classe [`PreviewOptions`](../previewoptions) entraînant la fermeture du flux de sortie. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Initialise une nouvelle instance de la classe [`PreviewOptions`](../previewoptions) entraînant le renvoi du flux de sortie au client pour une utilisation ultérieure. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CreatePageStream](../../groupdocs.parser.options/previewoptions/createpagestream) { get; set; } | Obtient ou définit une instance du délégué de création du flux de page. |
| [Dpi](../../groupdocs.parser.options/previewoptions/dpi) { get; set; } | Obtient ou définit un dpi. |
| [Height](../../groupdocs.parser.options/previewoptions/height) { get; set; } | Obtient ou définit la hauteur de l'aperçu de page. |
| [PageNumbers](../../groupdocs.parser.options/previewoptions/pagenumbers) { get; set; } | Obtient ou définit un tableau de numéros de page pour générer les aperçus. |
| [PreviewFormat](../../groupdocs.parser.options/previewoptions/previewformat) { get; set; } | Obtient ou définit le format de l'image d'aperçu. |
| [PreviewPageRender](../../groupdocs.parser.options/previewoptions/previewpagerender) { get; set; } | Obtient ou définit une instance du délégué d'informations de rendu de l'aperçu de page. |
| [ReleasePageStream](../../groupdocs.parser.options/previewoptions/releasepagestream) { get; set; } | Obtient ou définit une instance du délégué de complétion de l'aperçu de page. |
| [Width](../../groupdocs.parser.options/previewoptions/width) { get; set; } | Obtient ou définit la largeur de l'aperçu de page. |

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
