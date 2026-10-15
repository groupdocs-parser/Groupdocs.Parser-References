---
title: "HighlightOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "विकल्प प्रदान करता है जो खोज परिदृश्यों में पाए गए पाठ के आसपास एक ब्लॉक टेक्स्ट को हाइलाइट करने के लिए उपयोग किए जाते हैं।"
type: docs
weight: 360
url: /hi/net/groupdocs.parser.options/highlightoptions/
---

## HighlightOptions class

खोज परिदृश्यों में पाए गए टेक्स्ट के आसपास एक ब्लॉक (हाइलाइट) निकालने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public sealed class HighlightOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)() | एक नया उदाहरण प्रारंभ करता है [`HighlightOptions`](../highlightoptions) क्लास का, जिसका उपयोग निश्चित लंबाई का हाइलाइट निकालने के लिए किया जाता है। |
| [HighlightOptions](highlightoptions#constructor_1)(int) | एक नया उदाहरण प्रारंभ करता है [`HighlightOptions`](../highlightoptions) क्लास का, जिसका उपयोग निश्चित लंबाई का हाइलाइट निकालने के लिए किया जाता है। |
| [HighlightOptions](highlightoptions#constructor_2)(int?, bool) | एक नया उदाहरण प्रारंभ करता है [`HighlightOptions`](../highlightoptions) क्लास का, जिसका उपयोग पंक्ति-सीमित हाइलाइट निकालने के लिए किया जाता है। |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int) | एक नया उदाहरण प्रारंभ करता है [`HighlightOptions`](../highlightoptions) क्लास का, जिसका उपयोग निश्चित शब्द गिनती वाले हाइलाइट निकालने के लिए किया जाता है। |
| [HighlightOptions](highlightoptions#constructor_4)(int?, int?, bool) | एक नया उदाहरण प्रारंभ करता है [`HighlightOptions`](../highlightoptions) क्लास का। |

## गुण

| नाम | विवरण |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; set; } | एक मान प्राप्त करता है जो दर्शाता है कि हाइलाइट निष्कर्षण टेक्स्ट लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं। |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; set; } | अधिकतम टेक्स्ट लंबाई प्राप्त करता है। |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; set; } | अधिकतम शब्द गणना प्राप्त करता है। |

### टिप्पणियाँ

एक उदाहरण [`HighlightOptions`](../highlightoptions) क्लास का पैरामीटर के रूप में [`GetHighlight`](../../groupdocs.parser/parser/gethighlight) मेथड में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
