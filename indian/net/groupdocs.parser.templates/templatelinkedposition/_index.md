---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "लिंक्ड फ़ील्ड का उपयोग करने वाली टेम्प्लेट फ़ील्ड स्थिति प्रदान करता है।"
type: docs
weight: 110
url: /hi/net/groupdocs.parser.templates/templatelinkedposition/
---

## TemplateLinkedPosition class

लिंक्ड फ़ील्ड का उपयोग करने वाली टेम्प्लेट फ़ील्ड स्थिति प्रदान करता है।

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | [`TemplateLinkedPosition`](../templatelinkedposition) क्लास का नया उदाहरण आरंभ करता है। |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | [`TemplateLinkedPosition`](../templatelinkedposition) क्लास का नया उदाहरण UPPER CASE लिंक्ड फ़ील्ड नाम के साथ आरंभ करता है। |
| [TemplateLinkedPosition](templatelinkedposition#constructor_2)(string, Size, TemplateLinkedPositionEdges, bool, bool) | [`TemplateLinkedPosition`](../templatelinkedposition) क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | [`SearchArea`](./searcharea) को लिंक्ड फ़ील्ड आकार द्वारा स्केल किया गया है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | फ़ील्ड खोजे जाने वाले लिंक्ड फ़ील्ड के किनारे प्राप्त करता है। |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | लिंक्ड फ़ील्ड का नाम प्राप्त करता है। |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | फ़ील्ड खोजे जाने वाले क्षेत्र का आकार प्राप्त करता है। |

### Examples

निम्न उदाहरण कोड दिखाता है उस स्थिति के लिए जब यह ज्ञात हो कि चालान संख्या वाला फ़ील्ड "Invoice number" स्ट्रिंग के दाएँ पक्ष में स्थित है, इस कोड का उपयोग किया जाता है:

```csharp
// "Invoice Number" टेक्स्ट खोजने के लिए एक regex टेम्प्लेट फ़ील्ड बनाएं
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// "Invoice" फ़ील्ड से संबंधित एक टेम्प्लेट फ़ील्ड बनाएं और उसके दाएँ स्थित मान निकालें
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### संबंधित देखें

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
