---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "रेगुलर एक्सप्रेशन का उपयोग करने वाली टेम्प्लेट फ़ील्ड स्थिति प्रदान करता है।"
type: docs
weight: 150
url: /hi/net/groupdocs.parser.templates/templateregexposition/
---

## TemplateRegexPosition class

रेगुलर एक्सप्रेशन का उपयोग करने वाली टेम्प्लेट फ़ील्ड स्थिति प्रदान करता है।

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | एक नया उदाहरण प्रारंभ करता है [`TemplateRegexPosition`](../templateregexposition) क्लास का। |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | एक नया उदाहरण प्रारंभ करता है [`TemplateRegexPosition`](../templateregexposition) क्लास का। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | नियमित अभिव्यक्ति प्राप्त करता है। |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या पाठ केस अनदेखा नहीं किया गया है। |

### Examples

निम्न उदाहरण दर्शाता है कि यदि दस्तावेज़ में "Invoice Number INV-12345" हो तो टेम्प्लेट फ़ील्ड को निम्न प्रकार परिभाषित किया जा सकता है:

```csharp
// "InvoiceNumber" नाम के साथ एक regex टेम्प्लेट फ़ील्ड बनाएं
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

इस मामले में मान के रूप में पूरी स्ट्रिंग निकाली जाती है। स्ट्रिंग के केवल एक भाग को निकालने के लिए नियमित अभिव्यक्ति समूह "value" का उपयोग किया जाता है:

```csharp
// "InvoiceNumber" नाम के साथ "value" समूह वाला regex टेम्प्लेट फ़ील्ड बनाएं
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

इस मामले में मान के रूप में "INV-3337" स्ट्रिंग निकाली जाती है।

### संबंधित देखें

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
