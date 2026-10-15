---
title: "OcrOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "OCR कनेक्टर के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 450
url: /hi/net/groupdocs.parser.options/ocroptions/
---

## OcrOptions class

OCR कनेक्टर के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public class OcrOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OcrOptions](ocroptions#constructor)() | एक आयताकार क्षेत्र के साथ [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |
| [OcrOptions](ocroptions#constructor_5)(OcrEventHandler) | [`OcrEventHandler`](../ocreventhandler) ऑब्जेक्ट के साथ [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |
| [OcrOptions](ocroptions#constructor_6)(PagePreviewOptions) | एक आयताकार क्षेत्र के साथ [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |
| [OcrOptions](ocroptions#constructor_1)(Rectangle) | एक आयताकार क्षेत्र के साथ [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |
| [OcrOptions](ocroptions#constructor_2)(Rectangle, OcrEventHandler) | आयताकार क्षेत्र और [`OcrEventHandler`](../ocreventhandler) ऑब्जेक्ट के साथ [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |
| [OcrOptions](ocroptions#constructor_3)(Rectangle, OcrEventHandler, PagePreviewOptions, bool) | [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |
| [OcrOptions](ocroptions#constructor_4)(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) | [`OcrOptions`](../ocroptions) क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Handler](../../groupdocs.parser.options/ocroptions/handler) { get; set; } | OCR घटनाओं को पकड़ने के लिए इवेंट हैंडलर प्राप्त करता है। |
| [Language](../../groupdocs.parser.options/ocroptions/language) { get; set; } | OCR के लिए उपयोग की जाने वाली भाषा प्राप्त करता है या सेट करता है। पहचान के दौरान उपयोग किए जाने वाले वर्णमाला को निर्धारित करता है। डिफ़ॉल्ट रूप से अंग्रेज़ी उपयोग की जाती है। |
| [PagePreviewOptions](../../groupdocs.parser.options/ocroptions/pagepreviewoptions) { get; set; } | दस्तावेज़ पृष्ठ पूर्वावलोकन विकल्प प्राप्त करता है। |
| [Rectangle](../../groupdocs.parser.options/ocroptions/rectangle) { get; set; } | पाठ पहचान के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र को सीमित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
| [UseSpellChecker](../../groupdocs.parser.options/ocroptions/usespellchecker) { get; set; } | स्पेल चेकर के उपयोग को दर्शाने वाला मान प्राप्त करता है। |

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
