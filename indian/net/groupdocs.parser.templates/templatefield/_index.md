---
title: "TemplateField"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "टेम्प्लेट टेक्स्ट फ़ील्ड प्रदान करता है।"
type: docs
weight: 80
url: /hi/net/groupdocs.parser.templates/templatefield/
---

## TemplateField class

टेम्प्लेट टेक्स्ट फ़ील्ड प्रदान करता है।

```csharp
public sealed class TemplateField : TemplateItem
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | [`TemplateField`](../templatefield) क्लास का नया उदाहरण आरंभ करता है। |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, double?) | [`TemplateField`](../templatefield) क्लास का नया उदाहरण आरंभ करता है। |
| [TemplateField](templatefield#constructor_2)(TemplatePosition, string, double?, bool) | [`TemplateField`](../templatefield) क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [IsHidden](../../groupdocs.parser.templates/templatefield/ishidden) { get; set; } | छिपे हुए टेम्पलेट फ़ील्ड फ़्लैग को प्राप्त करता है या सेट करता है। |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | टेम्प्लेट आइटम का नाम प्राप्त करता है। |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई प्राप्त करता है। |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | दस्तावेज़ पृष्ठ पर टेम्पलेट फ़ील्ड को खोजने के तरीके का वर्णन करने वाले मान को प्राप्त करता है। |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | एक बूलियन मान प्राप्त करता है जो दर्शाता है कि क्या `Name` को UPPER CASE में परिवर्तित किया गया था। |
| [Value](../../groupdocs.parser.templates/templatefield/value) { get; set; } | टेम्पलेट फ़ील्ड का मान प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatefield/scale)(double) | इस टेम्प्लेट आइटम को दिए गए फैक्टर से स्केल करता है। |

### टिप्पणियाँ

पृष्ठ पर उसकी स्थिति द्वारा टेक्स्ट फ़ील्ड परिभाषित किए जाते हैं। टेक्स्ट फ़ील्ड को परिभाषित करने के तीन तरीके हैं:

* [`Using the rectangular area`](../templatefixedposition)
* [`Using the regular expression`](../templateregexposition)
* [`Using the linked field`](../templatelinkedposition)

### संबंधित देखें

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
