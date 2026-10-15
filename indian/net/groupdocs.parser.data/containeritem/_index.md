---
title: "ContainerItem"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "ज़िप आर्काइव इकाई, ईमेल अटैचमेंट, पीडीएफ पोर्टफ़ोलियो आइटम आदि जैसे कंटेनर आइटम को दर्शाता है।"
type: docs
weight: 720
url: /hi/net/groupdocs.parser.data/containeritem/
---

## ContainerItem class

ज़िप आर्काइव एंटिटी, ईमेल अटैचमेंट, PDF पोर्टफ़ोलियो आइटम आदि जैसे कंटेनर आइटम को दर्शाता है।

```csharp
public sealed class ContainerItem
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | आइटम की डायरेक्टरी प्राप्त करता है। |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | आइटम का पूर्ण पथ प्राप्त करता है। |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | मेटाडाटा आइटमों का संग्रह प्राप्त करता है। |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | आइटम का नाम प्राप्त करता है। |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | आइटम का आकार प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | कंटेनर आइटम की फ़ाइल प्रकार का पता लगाता है। |
| [GetMetadataValue](../../groupdocs.parser.data/containeritem/getmetadatavalue)(string) | मेटाडाटा मान प्राप्त करता है। |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | आइटम सामग्री के लिए [`Parser`](../../groupdocs.parser/parser) ऑब्जेक्ट बनाता है। |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | आइटम सामग्री के लिए [`LoadOptions`](../../groupdocs.parser.options/loadoptions) के साथ [`Parser`](../../groupdocs.parser/parser) ऑब्जेक्ट बनाता है। |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | आइटम सामग्री के लिए [`LoadOptions`](../../groupdocs.parser.options/loadoptions) और [`ParserSettings`](../../groupdocs.parser.options/parsersettings) के साथ [`Parser`](../../groupdocs.parser/parser) ऑब्जेक्ट बनाता है। |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | आइटम सामग्री की स्ट्रीम खोलता है। |

### टिप्पणियाँ

[`ContainerItem`](../containeritem) क्लास का एक इंस्टेंस [`GetContainer`](../../groupdocs.parser/parser/getcontainer) मेथड के रिटर्न वैल्यू के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

### संबंधित देखें

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
