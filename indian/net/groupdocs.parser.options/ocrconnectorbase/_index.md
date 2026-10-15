---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "OCR कार्यक्षमता प्रदान करता है।"
type: docs
weight: 430
url: /hi/net/groupdocs.parser.options/ocrconnectorbase/
---

## OcrConnectorBase class

OCR कार्यक्षमता प्रदान करता है।

```csharp
public abstract class OcrConnectorBase
```

## गुण

| नाम | विवरण |
| --- | --- |
| virtual [IsTextAreasSupported](../../groupdocs.parser.options/ocrconnectorbase/istextareassupported) { get; } | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट एरिया निष्कर्षण समर्थित है या नहीं। |
| virtual [IsTextSupported](../../groupdocs.parser.options/ocrconnectorbase/istextsupported) { get; } | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट निष्कर्षण समर्थित है या नहीं। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| virtual [RecognizeText](../../groupdocs.parser.options/ocrconnectorbase/recognizetext#recognizetext)(Stream, OcrOptions) | *imageStream* स्ट्रीम से टेक्स्ट को पहचानें। |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas)(Stream, Page, OcrOptions) | *imageStream* स्ट्रीम से टेक्स्ट एरिया को पहचानें। |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas_3)(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) | *imageStream* स्ट्रीम से टेक्स्ट एरिया को पहचानें। |

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
