---
title: "RecognizeTextAreas"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "imageStream स्ट्रीम से टेक्स्ट क्षेत्रों को पहचानें।"
type: docs
weight: 40
url: /hi/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---

## RecognizeTextAreas(Stream, Page, OcrOptions) {#recognizetextareas}

*imageStream* स्ट्रीम से टेक्स्ट एरिया को पहचानें।

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, Page page, 
    OcrOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| imageStream | Stream | दस्तावेज़ पृष्ठ की छवि प्रतिनिधित्व। |
| page | Page | दस्तावेज़ पृष्ठ। |
| options | OcrOptions | OCR विकल्प। |

### रिटर्न वैल्यू

[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह; यदि टेक्स्ट क्षेत्रों की पहचान समर्थित नहीं है तो `null`।

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## RecognizeTextAreas(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) {#recognizetextareas_3}

*imageStream* स्ट्रीम से टेक्स्ट एरिया को पहचानें।

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, 
    IEnumerable<Rectangle> rectangles, string allowedSymbols, Page page, OcrOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| imageStream | Stream | दस्तावेज़ पृष्ठ की छवि प्रतिनिधित्व। |
| rectangles | IEnumerable`1 | आयताकार क्षेत्रों का संग्रह जो OCR कार्यक्षमता को सीमित करता है। |
| allowedSymbols | स्ट्रिंग | OCR द्वारा अनुमत प्रतीकों का फ़िल्टर। |
| page | Page | दस्तावेज़ पृष्ठ। |
| options | OcrOptions | OCR विकल्प। |

### रिटर्न वैल्यू

[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह; यदि टेक्स्ट क्षेत्रों की पहचान समर्थित नहीं है तो `null`।

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
