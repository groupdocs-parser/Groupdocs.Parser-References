---
title: ContainerItem
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: ज़प संग्रह इकई ईमेल अटैचमेंट पडएफ पर्टफलय आइटम जैसे कंटेनर आइटम क प्रतनधत्व करत है
type: docs
weight: 10
url: /hi/net/groupdocs.parser.data/containeritem/
---
## ContainerItem class

ज़िप संग्रह इकाई, ईमेल अटैचमेंट, पीडीएफ पोर्टफोलियो आइटम जैसे कंटेनर आइटम का प्रतिनिधित्व करता है।

```csharp
public sealed class ContainerItem
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | आइटम की निर्देशिका प्राप्त करता है। |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | आइटम का पूरा पथ प्राप्त करता है। |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | मेटाडेटा आइटम का संग्रह प्राप्त करता है। |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | आइटम का नाम प्राप्त करता है। |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | आइटम का आकार प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | कंटेनर आइटम के फ़ाइल प्रकार का पता लगाता है। |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | बनाता है[`Parser`](../../groupdocs.parser/parser) आइटम सामग्री के लिए ऑब्जेक्ट. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | बनाता है[`Parser`](../../groupdocs.parser/parser) आइटम सामग्री के लिए वस्तु[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | बनाता है[`Parser`](../../groupdocs.parser/parser) आइटम सामग्री के लिए वस्तु[`LoadOptions`](../../groupdocs.parser.options/loadoptions) और[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | आइटम सामग्री की स्ट्रीम खोलता है. |

### टिप्पणियों

का एक उदाहरण[`ContainerItem`](../containeritem) वर्ग का उपयोग वापसी मान के रूप में किया जाता है[`GetContainer`](../../groupdocs.parser/parser/getcontainer) तरीका। वहां उपयोग के उदाहरण देखें.

### यह सभी देखें

* नाम स्थान [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* सभा [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
