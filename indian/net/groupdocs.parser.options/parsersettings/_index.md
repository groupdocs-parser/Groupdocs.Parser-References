---
title: "ParserSettings"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले सेटिंग्स प्रदान करता है।"
type: docs
weight: 540
url: /hi/net/groupdocs.parser.options/parsersettings/
---

## ParserSettings class

डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले सेटिंग्स प्रदान करता है।

```csharp
public sealed class ParserSettings
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ParserSettings](parsersettings#constructor)(ExternalResourceHandler) | एक नया उदाहरण प्रारंभ करता है [`ParserSettings`](../parsersettings) क्लास का, जिसमें External Resource Handler शामिल है। |
| [ParserSettings](parsersettings#constructor_1)(ILogger) | एक नया उदाहरण प्रारंभ करता है [`ParserSettings`](../parsersettings) क्लास का, जिसमें logger शामिल है। |
| [ParserSettings](parsersettings#constructor_4)(OcrConnectorBase) | एक नया उदाहरण प्रारंभ करता है [`ParserSettings`](../parsersettings) क्लास का, जिसमें OCR Connector शामिल है। |
| [ParserSettings](parsersettings#constructor_2)(ILogger, OcrConnectorBase) | एक नया उदाहरण प्रारंभ करता है [`ParserSettings`](../parsersettings) क्लास का, जिसमें logger और OCR Connector शामिल हैं। |
| [ParserSettings](parsersettings#constructor_3)(ILogger, OcrConnectorBase, ExternalResourceHandler) | एक नया उदाहरण प्रारंभ करता है [`ParserSettings`](../parsersettings) क्लास का, जिसमें logger, OCR Connector और External Resource Handler शामिल हैं। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ExternalResourceHandler](../../groupdocs.parser.options/parsersettings/externalresourcehandler) { get; } | बाहरी संसाधनों के हैंडलर को प्राप्त करता है। |
| [Logger](../../groupdocs.parser.options/parsersettings/logger) { get; } | डेटा निष्कर्षण के दौरान घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किया जाने वाला logger प्राप्त करता है। |
| [OcrConnector](../../groupdocs.parser.options/parsersettings/ocrconnector) { get; } | OCR कार्यक्षमता प्रदान करने के लिए उपयोग किया जाने वाला OCR Connector प्राप्त करता है। |

### टिप्पणियाँ

**Learn more:**

* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
