---
title: "PageTextArea"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "पृष्ठ टेक्स्ट क्षेत्र दर्शाता है जो टेम्प्लेट द्वारा पार्सिंग या फ़ॉर्म पार्सिंग कार्यक्षमता में टेक्स्ट मान को दर्शाने के लिए उपयोग होता है।"
type: docs
weight: 860
url: /hi/net/groupdocs.parser.data/pagetextarea/
---

## PageTextArea class

पृष्ठ टेक्स्ट क्षेत्र दर्शाता है जो टेम्प्लेट द्वारा पार्सिंग या फ़ॉर्म पार्सिंग कार्यक्षमता में टेक्स्ट मान को दर्शाने के लिए उपयोग होता है।

```csharp
public sealed class PageTextArea : PageArea
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | [`PageTextArea`](../pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है। |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | [`PageTextArea`](../pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है। |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | [`PageTextArea`](../pagetextarea) क्लास का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | चाइल्ड टेक्स्ट पेज क्षेत्रों का संग्रह प्राप्त करता है। |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | बेस लाइन प्राप्त करता है। |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | दस्तावेज़ पृष्ठ की जानकारी जैसे पृष्ठ सूचकांक और पृष्ठ आकार प्राप्त करता है। |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | आयताकार क्षेत्र प्राप्त करता है। |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | पाठ प्राप्त करता है। |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | फ़ॉन्ट आकार, फ़ॉन्ट नाम आदि जैसी टेक्स्ट शैली प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | इस उदाहरण का मान स्ट्रिंग में परिवर्तित करता है। |

### टिप्पणियाँ

निम्नलिखित विधियों के रिटर्न मान के रूप में [`PageTextArea`](../pagetextarea) क्लास का एक उदाहरण उपयोग किया जाता है:

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

इसके अलावा, [`PageTextArea`](../pagetextarea) क्लास का एक उदाहरण [`PageArea`](../fielddata/pagearea) प्रॉपर्टी के मान के रूप में उपयोग किया जाता है।

वहाँ उपयोग के उदाहरण देखें।

टेक्स्ट एरिया एकल या संयुक्त हो सकता है। पहले मामले में इसमें वह टेक्स्ट होता है जो आयताकार क्षेत्र द्वारा सीमित होता है। दूसरे मामले में इसमें अन्य टेक्स्ट एरिया होते हैं; टेक्स्ट और टेबल गुण चाइल्ड टेक्स्ट एरिया द्वारा गणना किए जाते हैं।

### संबंधित देखें

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
