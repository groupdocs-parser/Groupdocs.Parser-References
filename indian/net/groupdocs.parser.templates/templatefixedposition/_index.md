---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "आयताकार क्षेत्र द्वारा परिभाषित टेम्प्लेट फ़ील्ड स्थिति प्रदान करता है।"
type: docs
weight: 90
url: /hi/net/groupdocs.parser.templates/templatefixedposition/
---

## TemplateFixedPosition class

आयताकार क्षेत्र द्वारा परिभाषित टेम्प्लेट फ़ील्ड स्थिति प्रदान करता है।

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | [`TemplateFixedPosition`](../templatefixedposition) क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | टेम्प्लेट फ़ील्ड को शामिल करने वाला आयताकार क्षेत्र प्राप्त करता है। |

### Examples

फ़ील्ड स्थिति को परिभाषित करने का यह सबसे सरल तरीका है। इसमें पृष्ठ पर एक आयताकार क्षेत्र सेट करना आवश्यक है जो फ़ील्ड मान को सीमित करता है। आयताकार क्षेत्र में (भले ही आंशिक रूप से) शामिल सभी टेक्स्ट को मान के रूप में निकाला जाएगा:

```csharp
// "Address" नाम के साथ एक स्थिर टेम्प्लेट फ़ील्ड बनाएं जो स्थिति (35, 160) पर एक आयत द्वारा सीमित है और आकार (110, 20) है
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### संबंधित देखें

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
