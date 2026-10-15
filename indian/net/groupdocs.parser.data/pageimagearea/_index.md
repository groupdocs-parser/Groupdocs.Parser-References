---
title: "PageImageArea"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "पृष्ठ इमेज क्षेत्र दर्शाता है जो टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में पृष्ठ पर इमेज को दर्शाने के लिए या ईमेल या ज़िप आर्काइव से निकाली गई इमेज अटैचमेंट को दर्शाने के लिए उपयोग होता है।"
type: docs
weight: 830
url: /hi/net/groupdocs.parser.data/pageimagearea/
---

## PageImageArea class

पृष्ठ इमेज क्षेत्र दर्शाता है जो टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में पृष्ठ पर इमेज को दर्शाने के लिए या ईमेल या ज़िप आर्काइव से निकाली गई इमेज अटैचमेंट को दर्शाने के लिए उपयोग होता है।

```csharp
public sealed class PageImageArea : PageArea
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | [`PageImageArea`](../pageimagearea) क्लास का नया उदाहरण प्रारंभ करता है। |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | [`PageImageArea`](../pageimagearea) क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | छवि का फ़ॉर्मेट प्राप्त करता है। |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | दस्तावेज़ पृष्ठ की जानकारी जैसे पृष्ठ सूचकांक और पृष्ठ आकार प्राप्त करता है। |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | आयताकार क्षेत्र प्राप्त करता है। |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | छवि का घूर्णन कोण प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | छवि स्ट्रीम लौटाता है। |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | विभिन्न प्रारूप में छवि स्ट्रीम लौटाता है। |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | छवि को फ़ाइल में सहेजता है। |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | छवि को विभिन्न प्रारूप में फ़ाइल में सहेजता है। |

### टिप्पणियाँ

निम्नलिखित विधियों के रिटर्न मान के रूप में [`PageImageArea`](../pageimagearea) क्लास का एक उदाहरण उपयोग किया जाता है:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

वहाँ उपयोग के उदाहरण देखें।

### संबंधित देखें

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
