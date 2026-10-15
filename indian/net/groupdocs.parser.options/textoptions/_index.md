---
title: "TextOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "पाठ निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 610
url: /hi/net/groupdocs.parser.options/textoptions/
---

## TextOptions class

पाठ निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public sealed class TextOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TextOptions](textoptions#constructor)() | [`TextOptions`](../textoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [TextOptions](textoptions#constructor_1)(bool) | [`TextOptions`](../textoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [TextOptions](textoptions#constructor_2)(bool, bool) | OCR उपयोग विकल्प के साथ [`TextOptions`](../textoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [TextOptions](textoptions#constructor_3)(bool, bool, OcrOptions) | एक नया उदाहरण प्रारंभ करता है [`TextOptions`](../textoptions) क्लास का, जिसमें OCR विकल्प सेट करने की क्षमता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [IncludeAnnotations](../../groupdocs.parser.options/textoptions/includeannotations) { get; set; } | ऐनोटेशन शामिल हैं या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान `false` है। |
| [OcrOptions](../../groupdocs.parser.options/textoptions/ocroptions) { get; set; } | OCR कार्यक्षमता के अतिरिक्त विकल्प प्राप्त करता है। |
| [UseOcr](../../groupdocs.parser.options/textoptions/useocr) { get; set; } | यह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट निकालने के लिए OCR कनेक्टर उपयोग किया गया है या नहीं। |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; set; } | यह मान प्राप्त करता है जो दर्शाता है कि रॉ मोड उपयोग किया गया है या नहीं। |

### टिप्पणियाँ

`[`TextOptions`](../textoptions)` क्लास का एक उदाहरण [`GetText`](../../groupdocs.parser/parser/gettext) और [`GetText`](../../groupdocs.parser/parser/gettext) मेथड्स में पैरामीटर के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

यह टेक्स्ट निष्कर्षण के रॉ मोड को निर्दिष्ट करने के लिए उपयोग किया जाता है। इस मोड में टेक्स्ट असटीक तरीके से निकाला जाता है लेकिन मानक मोड की तुलना में तेज़ होता है। यदि रॉ मोड दस्तावेज़ फ़ॉर्मेट का समर्थन नहीं करता, तो यह पैरामीटर अनदेखा कर दिया जाता है और मानक मोड उपयोग किया जाता है।

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
