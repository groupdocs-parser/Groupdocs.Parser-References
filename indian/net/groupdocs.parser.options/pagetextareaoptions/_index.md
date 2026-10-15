---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "पृष्ठ पाठ क्षेत्रों के निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 520
url: /hi/net/groupdocs.parser.options/pagetextareaoptions/
---

## PageTextAreaOptions class

पृष्ठ पाठ क्षेत्रों के निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)() | OCR उपयोग विकल्प के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool) | OCR उपयोग विकल्प के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string) | नियमित अभिव्यक्ति के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का नया उदाहरण आरंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(bool, OcrOptions) | OCR विकल्प सेट करने की क्षमता के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_6)(string, Rectangle) | नियमित अभिव्यक्ति और आयताकार क्षेत्र के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का नया उदाहरण आरंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_7)(string, Rectangle, double) | नियमित अभिव्यक्ति, आयताकार क्षेत्र और अनदेखी सीमा के आकार के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का नया उदाहरण आरंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, bool, bool, bool, Rectangle) | `[`PageTextAreaOptions`](../pagetextareaoptions)` क्लास का नया उदाहरण आरंभ करता है। |
| [PageTextAreaOptions](pagetextareaoptions#constructor_5)(string, bool, bool, bool, Rectangle, double) | अनदेखी सीमा के आकार के साथ [`PageTextAreaOptions`](../pagetextareaoptions) क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; set; } | नियमित अभिव्यक्ति प्राप्त करता है। |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या पाठ स्वरूपण अनदेखा किया गया है। |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या पाठ केस अनदेखा नहीं किया गया है। |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; set; } | OCR कार्यक्षमता के अतिरिक्त विकल्प प्राप्त करता है। |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | पेज क्षेत्रों को समाहित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखा किए जाने वाले बॉर्डर का आकार प्राप्त करता है। यह टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या खंड एकीकृत हैं। |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या OCR कार्यक्षमता का उपयोग करके पाठ क्षेत्रों को निकाला जाता है। |

### टिप्पणियाँ

`[`PageTextAreaOptions`](../pagetextareaoptions)` क्लास का एक उदाहरण [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) और [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) विधियों में पैरामीटर के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें। **Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### संबंधित देखें

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
