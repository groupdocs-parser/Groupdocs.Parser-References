---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "पृष्ठ कैसे रेंडर किया जाता है, इसकी जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 500
url: /hi/net/groupdocs.parser.options/pagerenderinfo/
---

## PageRenderInfo class

पृष्ठ कैसे रेंडर किया जाता है, इसकी जानकारी का प्रतिनिधित्व करता है।

```csharp
public sealed class PageRenderInfo
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageRenderInfo](pagerenderinfo)(int, int, int) | एक नया उदाहरण प्रारंभ करता है [`PageRenderInfo`](../pagerenderinfo) क्लास का। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ColumnCount](../../groupdocs.parser.options/pagerenderinfo/columncount) { get; } | टाइल कॉलम की कुल संख्या प्राप्त करें। |
| [PageNumber](../../groupdocs.parser.options/pagerenderinfo/pagenumber) { get; } | पृष्ठ संख्या प्राप्त करता है। |
| [RowCount](../../groupdocs.parser.options/pagerenderinfo/rowcount) { get; } | टाइल पंक्तियों की कुल संख्या प्राप्त करें। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetColumn](../../groupdocs.parser.options/pagerenderinfo/getcolumn)(int) | वह कॉलम इंडेक्स लौटाता है जहाँ *tileIndex* वाली टाइल रखी गई है। |
| [GetRow](../../groupdocs.parser.options/pagerenderinfo/getrow)(int) | वह पंक्ति इंडेक्स लौटाता है जहाँ *tileIndex* वाली टाइल रखी गई है। |

### टिप्पणियाँ

कुछ दस्तावेज़ (जैसे स्प्रेडशीट) को एक पृष्ठ को एकल छवि के रूप में रेंडर करना संभव नहीं होता। ऐसे दस्तावेज़ों के लिए पृष्ठ को टाइलों के सेट के रूप में रेंडर किया जाता है। ये टाइलें आयताकार तालिका में रखी जाती हैं।

[`RowCount`](./rowcount) and [`ColumnCount`](./columncount) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
