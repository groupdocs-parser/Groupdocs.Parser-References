---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "तालिका डिटेक्शन एल्गोरिदम के लिए पैरामीटर प्रदान करता है।"
type: docs
weight: 180
url: /hi/net/groupdocs.parser.templates/templatetableparameters/
---

## TemplateTableParameters class

तालिका डिटेक्शन एल्गोरिदम के लिए पैरामीटर प्रदान करता है।

```csharp
public sealed class TemplateTableParameters
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | [`TemplateTableParameters`](../templatetableparameters) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | [`TemplateTableParameters`](../templatetableparameters) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | टेबल में मर्ज किए गए सेल्स हैं या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | टेबल कॉलमों की न्यूनतम संख्या प्राप्त करता है। |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | टेबल पंक्तियों की न्यूनतम संख्या प्राप्त करता है। |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | टेबल कॉलमों के बीच न्यूनतम स्पेस प्राप्त करता है। |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | टेबल को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | टेबल कॉलम विभाजकों को प्राप्त करता है। |

### टिप्पणियाँ

टेबल का पता लगाने के लिए दो एल्गोरिदम हैं:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

कुछ मामलों में जब एल्गोरिदम टेबल का पता नहीं लगा पाते या असटीक तरीके से करते हैं, तो [`TemplateTableLayout`](../templatetablelayout) क्लास का उपयोग किया जाता है।

### संबंधित देखें

* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
