---
title: "OcrConnectorBase"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Fournit la fonctionnalité OCR."
type: docs
weight: 430
url: /fr/net/groupdocs.parser.options/ocrconnectorbase/
---

## OcrConnectorBase class

Fournit la fonctionnalité OCR.

```csharp
public abstract class OcrConnectorBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [IsTextAreasSupported](../../groupdocs.parser.options/ocrconnectorbase/istextareassupported) { get; } | Obtient la valeur qui indique si l'extraction des zones de texte est prise en charge. |
| virtual [IsTextSupported](../../groupdocs.parser.options/ocrconnectorbase/istextsupported) { get; } | Obtient la valeur qui indique si l'extraction du texte est prise en charge. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [RecognizeText](../../groupdocs.parser.options/ocrconnectorbase/recognizetext#recognizetext)(Stream, OcrOptions) | Reconnaître un texte à partir du flux *imageStream*. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas)(Stream, Page, OcrOptions) | Reconnaître les zones de texte à partir du flux *imageStream*. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas_3)(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) | Reconnaître les zones de texte à partir du flux *imageStream*. |

### Voir aussi

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
