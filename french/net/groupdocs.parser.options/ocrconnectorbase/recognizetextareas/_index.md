---
title: RecognizeTextAreas
second_title: Référence de l'API GroupDocs.Parser pour .NET
description: Reconnaître les zones de texte à partirimageStream flux.
type: docs
weight: 20
url: /fr/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---
## OcrConnectorBase.RecognizeTextAreas method

Reconnaître les zones de texte à partir*imageStream* flux.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, int pageIndex, 
    Size pageSize, OcrOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| imageStream | Stream | La représentation d'image de la page du document. |
| pageIndex | Int32 | L'index des pages du document. |
| pageSize | Size | La taille de la page du document. |
| options | OcrOptions | Les options d'OCR. |

### Return_Value

Une collection de[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objets;`nul` si la reconnaissance des zones de texte n'est pas prise en charge.

### Voir également

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Size](../../../groupdocs.parser.data/size)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* espace de noms [GroupDocs.Parser.Options](../../ocrconnectorbase)
* Assemblée [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->