---
title: "RecognizeText"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "imageStream स्ट्रीम से पाठ को पहचानें।"
type: docs
weight: 30
url: /hi/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---

## OcrConnectorBase.RecognizeText method

*imageStream* स्ट्रीम से टेक्स्ट को पहचानें।

```csharp
public virtual string RecognizeText(Stream imageStream, OcrOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| imageStream | Stream | दस्तावेज़ पृष्ठ की छवि प्रतिनिधित्व। |
| options | OcrOptions | OCR विकल्प। |

### रिटर्न वैल्यू

एक स्ट्रिंग जो पहचाने गए पाठ का प्रतिनिधित्व करती है; `null` यदि पाठ पहचान समर्थित नहीं है।

### संबंधित देखें

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
