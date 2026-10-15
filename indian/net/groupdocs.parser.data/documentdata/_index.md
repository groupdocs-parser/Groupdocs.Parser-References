---
title: "DocumentData"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ का डेटा दर्शाता है। यह FieldData/fielddata ऑब्जेक्ट्स से बना होता है जो दस्तावेज़ से फ़ील्ड डेटा रखते हैं।"
type: docs
weight: 730
url: /hi/net/groupdocs.parser.data/documentdata/
---

## DocumentData class

दस्तावेज़ का डेटा दर्शाता है। यह [`FieldData`](../fielddata) ऑब्जेक्ट्स से बना है जो दस्तावेज़ से फ़ील्ड डेटा रखते हैं।

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | फ़ील्ड डेटा की कुल संख्या प्राप्त करता है। |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | इंडेक्स द्वारा फ़ील्ड डेटा प्राप्त करता है। |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | टेम्प्लेट प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | फ़ील्ड डेटा के लिए एक एन्यूमरेटर लौटाता है। |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | फ़ील्ड डेटा का संग्रह लौटाता है जहाँ नाम *fieldName* के बराबर हो। |

### टिप्पणियाँ

एक उदाहरण [`DocumentData`](../documentdata) क्लास का [`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) और [`ParseForm`](../../groupdocs.parser/parser/parseform) मेथड्स के रिटर्न वैल्यू के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

### संबंधित देखें

* class [FieldData](../fielddata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
