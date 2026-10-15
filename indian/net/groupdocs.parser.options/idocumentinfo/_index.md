---
title: "IDocumentInfo"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 370
url: /hi/net/groupdocs.parser.options/idocumentinfo/
---

## IDocumentInfo interface

दस्तावेज़ जानकारी का प्रतिनिधित्व करता है।

```csharp
public interface IDocumentInfo
```

## गुण

| नाम | विवरण |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | दस्तावेज़ प्रकार प्राप्त करता है। |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | दस्तावेज़ पृष्ठों की कुल संख्या प्राप्त करता है। |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | पृष्ठों के बारे में जानकारी प्राप्त करता है, जैसे कि इंडेक्स और पृष्ठ आकार। |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | दस्तावेज़ के कच्चे पृष्ठों की कुल संख्या प्राप्त करता है। |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | दस्तावेज़ का आकार बाइट्स में प्राप्त करता है। |

### टिप्पणियाँ

यह इंटरफ़ेस लागू करने वाले ऑब्जेक्ट्स को [`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo) मेथड द्वारा लौटाया जाता है। वहाँ उपयोग के उदाहरण देखें। **अधिक जानें:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
