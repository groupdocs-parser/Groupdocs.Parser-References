---
title: "TemplateTable"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "टेम्प्लेट तालिका प्रदान करता है।"
type: docs
weight: 160
url: /hi/net/groupdocs.parser.templates/templatetable/
---

## TemplateTable class

टेम्प्लेट तालिका प्रदान करता है।

```csharp
public sealed class TemplateTable : TemplateItem
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string) | [`TemplateTable`](../templatetable) क्लास का नया उदाहरण UPPER CASE नाम के साथ आरंभ करता है। |
| [TemplateTable](templatetable#constructor_3)(TemplateTableParameters, string) | [`TemplateTable`](../templatetable) क्लास का नया उदाहरण आरंभ करता है। |
| [TemplateTable](templatetable#constructor_1)(TemplateTableLayout, string, double?) | [`TemplateTable`](../templatetable) क्लास का नया उदाहरण UPPER CASE नाम के साथ आरंभ करता है। |
| [TemplateTable](templatetable#constructor_4)(TemplateTableParameters, string, double?) | [`TemplateTable`](../templatetable) क्लास का नया उदाहरण आरंभ करता है। |
| [TemplateTable](templatetable#constructor_2)(TemplateTableLayout, string, double?, bool) | [`TemplateTable`](../templatetable) क्लास का नया उदाहरण आरंभ करता है। |
| [TemplateTable](templatetable#constructor_5)(TemplateTableParameters, string, double?, bool) | [`TemplateTable`](../templatetable) क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | टेबल लेआउट प्राप्त करता है। |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | टेम्प्लेट आइटम का नाम प्राप्त करता है। |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई प्राप्त करता है। |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | स्वचालित मोड में टेबल का पता लगाने के पैरामीटर प्राप्त करता है। |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | एक बूलियन मान प्राप्त करता है जो दर्शाता है कि क्या `Name` को UPPER CASE में परिवर्तित किया गया था। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatetable/scale)(double) | इस टेम्प्लेट आइटम को दिए गए फैक्टर से स्केल करता है। |

### टिप्पणियाँ

टेबल को परिभाषित करने के दो तरीके हैं:

* Using [`TemplateTableLayout`](../templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [`TemplateTableParameters`](../templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](../templatetableparameters) class for more information.

### संबंधित देखें

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
