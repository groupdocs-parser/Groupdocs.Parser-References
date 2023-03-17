---
title: RecognizeTextAreas
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Textbereiche erkennen ausimageStream stream.
type: docs
weight: 20
url: /de/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---
## OcrConnectorBase.RecognizeTextAreas method

Textbereiche erkennen aus*imageStream* stream.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, int pageIndex, 
    Size pageSize, OcrOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageStream | Stream | Die Bilddarstellung der Dokumentseite. |
| pageIndex | Int32 | Der Seitenindex des Dokuments. |
| pageSize | Size | Die Größe der Dokumentseite. |
| options | OcrOptions | Die OCR-Optionen. |

### Rückgabewert

Eine Sammlung von[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) Gegenstände;`Null` wenn die Erkennung von Textbereichen nicht unterstützt wird.

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Size](../../../groupdocs.parser.data/size)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namensraum [GroupDocs.Parser.Options](../../ocrconnectorbase)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->