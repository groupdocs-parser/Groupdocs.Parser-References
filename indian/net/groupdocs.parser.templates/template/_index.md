---
title: "टेम्पलेट"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ पृष्ठ टेम्पलेट प्रदान करता है। इसमें TemplateItem./templateitem ऑब्जेक्ट्स शामिल हैं जो टेम्पलेट के आइटम जैसे टेक्स्ट फ़ील्ड और तालिका परिभाषाओं का प्रतिनिधित्व करते हैं।"
type: docs
weight: 50
url: /hi/net/groupdocs.parser.templates/template/
---

## Template class

दस्तावेज़ पृष्ठ टेम्पलेट प्रदान करता है। इसमें [`TemplateItem`](../templateitem) ऑब्जेक्ट्स शामिल हैं जो टेम्पलेट के आइटम जैसे टेक्स्ट फ़ील्ड और तालिका परिभाषाओं का प्रतिनिधित्व करते हैं।

```csharp
public sealed class Template : IEnumerable<TemplateItem>
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Template](template#constructor)(IEnumerable&lt;TemplateItem&gt;) | [`Template`](../template) क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [Template](template#constructor_1)(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) | [`Template`](../template) क्लास का नया इंस्टेंस टेम्पलेट विकल्पों के साथ प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../groupdocs.parser.templates/template/count) { get; } | टेम्पलेट आइटम्स की कुल संख्या प्राप्त करता है। |
| [IsOcrCompatible](../../groupdocs.parser.templates/template/isocrcompatible) { get; } | टेम्पलेट OCR के साथ संगत है या नहीं यह दर्शाने वाला मान प्राप्त करता है। |
| [Item](../../groupdocs.parser.templates/template/item) { get; } | इंडेक्स द्वारा टेम्पलेट आइटम प्राप्त करता है। |
| [Options](../../groupdocs.parser.templates/template/options) { get; } | टेम्पलेट विकल्प प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [Load](../../groupdocs.parser.templates/template/load#load)(Stream) | स्ट्रीम से टेम्पलेट लोड करता है। |
| static [Load](../../groupdocs.parser.templates/template/load#load_1)(string) | फ़ाइल से टेम्पलेट लोड करता है। |
| [GetEnumerator](../../groupdocs.parser.templates/template/getenumerator)() | टेम्पलेट आइटम्स के लिए एक एनेमरेटर लौटाता है। |
| [Save](../../groupdocs.parser.templates/template/save#save)(Stream) | टेम्पलेट को स्ट्रीम में सहेजता है। |
| [Save](../../groupdocs.parser.templates/template/save#save_1)(string) | टेम्पलेट को फ़ाइल में सहेजता है। |

### टिप्पणियाँ

**Learn more:**

* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)

### संबंधित देखें

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
