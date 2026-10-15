---
title: "RecognizeTextAreas"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Reconnaît les zones de texte à partir du flux imageStream."
type: docs
weight: 40
url: /fr/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---

## RecognizeTextAreas(Stream, Page, OcrOptions) {#recognizetextareas}

Reconnaître les zones de texte à partir du flux *imageStream*.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, Page page, 
    OcrOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageStream | Stream | La représentation image de la page du document. |
| page | Page | La page du document. |
| options | OcrOptions | Les options OCR. |

### Valeur de retour

Une collection d'objets [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ; `null` si la reconnaissance des zones de texte n'est pas prise en charge.

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## RecognizeTextAreas(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) {#recognizetextareas_3}

Reconnaître les zones de texte à partir du flux *imageStream*.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, 
    IEnumerable<Rectangle> rectangles, string allowedSymbols, Page page, OcrOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| imageStream | Stream | La représentation image de la page du document. |
| rectangles | IEnumerable`1 | La collection des zones rectangulaires qui limite la fonctionnalité OCR. |
| allowedSymbols | Chaîne | Le filtre des symboles autorisés par OCR. |
| page | Page | La page du document. |
| options | OcrOptions | Les options OCR. |

### Valeur de retour

Une collection d'objets [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ; `null` si la reconnaissance des zones de texte n'est pas prise en charge.

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
