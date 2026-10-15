---
title: "RecognizeText"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Erkenne einen Text aus dem imageStream-Stream."
type: docs
weight: 30
url: /de/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---

## OcrConnectorBase.RecognizeText method

Erkenne einen Text aus dem *imageStream*-Stream.

```csharp
public virtual string RecognizeText(Stream imageStream, OcrOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageStream | Stream | Die Bilddarstellung der Dokumentenseite. |
| options | OcrOptions | Die OCR-Optionen. |

### Rückgabewert

Ein String, der einen erkannten Text darstellt; `null`, wenn die Texterkennung nicht unterstützt wird.

### Siehe auch

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
