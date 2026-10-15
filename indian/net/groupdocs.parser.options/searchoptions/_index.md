---
title: "SearchOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "पाठ खोज के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 590
url: /hi/net/groupdocs.parser.options/searchoptions/
---

## SearchOptions class

पाठ खोज के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

```csharp
public sealed class SearchOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | डिफ़ॉल्ट मानों के साथ [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। विवरण के लिए टिप्पणी देखें। |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | हाइलाइट निष्कर्षण के बिना खोज करने के लिए उपयोग की जाने वाली [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | पृष्ठों द्वारा और हाइलाइट निष्कर्षण के बिना खोज करने के लिए उपयोग की जाने वाली [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए समान हाइलाइट विकल्पों के साथ खोज करने के लिए उपयोग की जाने वाली [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए हाइलाइट विकल्पों के साथ खोज करने के लिए उपयोग की जाने वाली [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [SearchOptions](searchoptions#constructor_6)(bool, bool, bool, int, HighlightOptions, HighlightOptions) | पृष्ठ सीमा के साथ [`SearchOptions`](../searchoptions) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; set; } | बाएँ हाइलाइट के विकल्प प्राप्त करता है। |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या पाठ केस अनदेखा नहीं किया गया है। |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या टेक्स्ट खोज पूरे शब्द द्वारा सीमित है। |
| [MaxPageIndex](../../groupdocs.parser.options/searchoptions/maxpageindex) { get; set; } | खोज के लिए पृष्ठ के अधिकतम इंडेक्स को दर्शाने वाला मान प्राप्त करता है। |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; set; } | दाएँ हाइलाइट के विकल्प प्राप्त करता है। |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या खोज पृष्ठों द्वारा की जाती है। |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है कि क्या नियमित अभिव्यक्ति उपयोग की गई है। |

### टिप्पणियाँ

एक [`SearchOptions`](../searchoptions) क्लास की इंस्टेंस को [`Search`](../../groupdocs.parser/parser/search) मेथड में पैरामीटर के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
