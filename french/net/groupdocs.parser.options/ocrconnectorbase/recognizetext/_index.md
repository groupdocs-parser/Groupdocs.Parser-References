---
title: "RecognizeText"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Reconnaître un texte à partir du flux imageStream."
type: docs
weight: 30
url: /fr/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---

## OcrConnectorBase.RecognizeText method

Reconnaître un texte à partir du flux *imageStream*.

```csharp
public virtual string RecognizeText(Stream imageStream, OcrOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageStream | Stream | La représentation image de la page du document. |
| options | OcrOptions | Les options OCR. |

### Valeur de retour

Une chaîne qui représente un texte reconnu ; `null` si la reconnaissance de texte n'est pas prise en charge.

### Voir aussi

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
