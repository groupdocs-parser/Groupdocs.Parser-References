---
title: "LoadOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "फ़ाइल खोलने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 420
url: /hi/net/groupdocs.parser.options/loadoptions/
---

## LoadOptions class

फ़ाइल खोलने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public sealed class LoadOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, जिसमें खाली [`Password`](./password), [`FileFormat`](./fileformat) Unknown के बराबर और डिफ़ॉल्ट एन्कोडिंग्स हैं। |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, जिसमें खाली [`Password`](./password) और डिफ़ॉल्ट एन्कोडिंग्स हैं। |
| [LoadOptions](loadoptions#constructor_5)(FileType) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, जिसमें खाली [`Password`](./password) और डिफ़ॉल्ट एन्कोडिंग्स हैं। |
| [LoadOptions](loadoptions#constructor_9)(string) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, जिसमें [`FileFormat`](./fileformat) Unknown के बराबर और डिफ़ॉल्ट एन्कोडिंग्स हैं। |
| [LoadOptions](loadoptions#constructor_10)(TimeSpan) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, *timeout* के साथ। |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, पासवर्ड और डिफ़ॉल्ट एन्कोडिंग्स के साथ। |
| [LoadOptions](loadoptions#constructor_6)(FileType, string) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, पासवर्ड और डिफ़ॉल्ट एन्कोडिंग्स के साथ। |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, कस्टम एन्कोडिंग्स के साथ। |
| [LoadOptions](loadoptions#constructor_7)(FileType, string, Encoding, Encoding) | एक नया उदाहरण प्रारंभ करता है [`LoadOptions`](../loadoptions) क्लास का, कस्टम एन्कोडिंग्स के साथ। |
| [LoadOptions](loadoptions#constructor_4)(FileFormat, string, Encoding, Encoding, TimeSpan) | एक नया उदाहरण प्रारंभ करता है पूरी तरह से अनुकूलित [`LoadOptions`](../loadoptions) क्लास का। |
| [LoadOptions](loadoptions#constructor_8)(FileType, string, Encoding, Encoding, TimeSpan) | एक नया उदाहरण प्रारंभ करता है पूरी तरह से अनुकूलित [`LoadOptions`](../loadoptions) क्लास का। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | डिफ़ॉल्ट ANSI एन्कोडिंग प्राप्त करता है, जिसका उपयोग एन्कोडिंग पहचान के लिए किया जाता है। |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | दस्तावेज़ की एन्कोडिंग प्राप्त करता है। |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | फ़ाइल फ़ॉर्मेट प्राप्त करता है। |
| [FileType](../../groupdocs.parser.options/loadoptions/filetype) { get; } | फ़ाइल प्रकार प्राप्त करता है। |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | पासवर्ड प्राप्त करता है। |
| [Timeout](../../groupdocs.parser.options/loadoptions/timeout) { get; } | वह मान प्राप्त करता है जो प्रतीक्षा करने वाले मिलीसेकंड की संख्या को दर्शाता है। |

### टिप्पणियाँ

इस क्लास का एक उदाहरण पैरामीटर के रूप में उपयोग किया जाता है [`Parser`](../../groupdocs.parser/parser) क्लास के कंस्ट्रक्टर्स में:

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

वहाँ उपयोग के उदाहरण देखें।

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
