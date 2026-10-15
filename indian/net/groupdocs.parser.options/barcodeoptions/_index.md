---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "बारकोड निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 200
url: /hi/net/groupdocs.parser.options/barcodeoptions/
---

## BarcodeOptions class

बारकोड निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public sealed class BarcodeOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [BarcodeOptions](barcodeoptions#constructor)() | डिफ़ॉल्ट मानों के साथ [`BarcodeOptions`](../barcodeoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [BarcodeOptions](barcodeoptions#constructor_1)(Rectangle) | आयताकार क्षेत्र के साथ [`BarcodeOptions`](../barcodeoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [BarcodeOptions](barcodeoptions#constructor_3)(QualityMode, QualityMode, params string[]) | गुणवत्ता सेटिंग्स और कोड प्रकारों के साथ [`BarcodeOptions`](../barcodeoptions) क्लास का नया उदाहरण आरंभ करता है। |
| [BarcodeOptions](barcodeoptions#constructor_2)(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) | `[`BarcodeOptions`](../barcodeoptions)` क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AllowIncorrectBarcodes](../../groupdocs.parser.options/barcodeoptions/allowincorrectbarcodes) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या गलत बारकोड की अनुमति है। |
| [BarcodeQuality](../../groupdocs.parser.options/barcodeoptions/barcodequality) { get; set; } | स्रोत बारकोड की गुणवत्ता प्राप्त करता है। |
| [CodeTypes](../../groupdocs.parser.options/barcodeoptions/codetypes) { get; set; } | पढ़ने के लिए बारकोड प्रकार प्राप्त करता है। |
| [Dimension](../../groupdocs.parser.options/barcodeoptions/dimension) { get; set; } | बारकोड न्यूनतम तत्व का न्यूनतम आकार प्राप्त करता है। |
| [ImageQuality](../../groupdocs.parser.options/barcodeoptions/imagequality) { get; set; } | स्रोत छवि की गुणवत्ता प्राप्त करता है। |
| [PagePreviewOptions](../../groupdocs.parser.options/barcodeoptions/pagepreviewoptions) { get; set; } | दस्तावेज़ पृष्ठ पूर्वावलोकन विकल्प प्राप्त करता है या सेट करता है। |
| [Rectangle](../../groupdocs.parser.options/barcodeoptions/rectangle) { get; set; } | पेज क्षेत्रों को समाहित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
