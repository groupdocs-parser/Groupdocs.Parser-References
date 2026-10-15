---
title: "SearchOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "SearchOptionsgroupdocs.parser.options/searchoptions क्लास का नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

[`SearchOptions`](../../searchoptions) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| matchWholeWord | Boolean | मान जो दर्शाता है कि क्या पाठ खोज पूर्ण शब्द द्वारा सीमित है। |
| useRegularExpression | Boolean | मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
| searchByPages | Boolean | मान जो दर्शाता है कि क्या खोज पृष्ठों द्वारा की जाती है। |
| leftHighlightOptions | HighlightOptions | बाएँ हाइलाइट के विकल्प। |
| rightHighlightOptions | HighlightOptions | दाएँ हाइलाइट के विकल्प। |

### संबंधित देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

पेज सीमा के साथ [`SearchOptions`](../../searchoptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| matchWholeWord | Boolean | मान जो दर्शाता है कि क्या पाठ खोज पूर्ण शब्द द्वारा सीमित है। |
| useRegularExpression | Boolean | मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
| maxPageIndex | Int32 | वह मान जो दर्शाता है कि खोज पृष्ठों द्वारा की जाती है। |
| leftHighlightOptions | HighlightOptions | बाएँ हाइलाइट के विकल्प। |
| rightHighlightOptions | HighlightOptions | दाएँ हाइलाइट के विकल्प। |

### संबंधित देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए हाइलाइट विकल्पों के साथ खोज करने हेतु [`SearchOptions`](../../searchoptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| matchWholeWord | Boolean | मान जो दर्शाता है कि क्या पाठ खोज पूर्ण शब्द द्वारा सीमित है। |
| useRegularExpression | Boolean | मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
| leftHighlightOptions | HighlightOptions | बाएँ हाइलाइट के विकल्प। |
| rightHighlightOptions | HighlightOptions | दाएँ हाइलाइट के विकल्प। |

### संबंधित देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए समान हाइलाइट विकल्पों के साथ खोज करने हेतु [`SearchOptions`](../../searchoptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| matchWholeWord | Boolean | मान जो दर्शाता है कि क्या पाठ खोज पूर्ण शब्द द्वारा सीमित है। |
| useRegularExpression | Boolean | मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
| highlightOptions | HighlightOptions | दोनों हाइलाइट्स के विकल्प। |

### संबंधित देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

हाइलाइट निष्कर्षण के बिना खोज के लिए उपयोग किया जाने वाला [`SearchOptions`](../../searchoptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| matchWholeWord | Boolean | मान जो दर्शाता है कि क्या पाठ खोज पूर्ण शब्द द्वारा सीमित है। |
| useRegularExpression | Boolean | मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |

### संबंधित देखें

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

पृष्ठों द्वारा खोज और हाइलाइट निष्कर्षण के बिना खोज के लिए उपयोग किया जाने वाला [`SearchOptions`](../../searchoptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| matchWholeWord | Boolean | मान जो दर्शाता है कि क्या पाठ खोज पूर्ण शब्द द्वारा सीमित है। |
| useRegularExpression | Boolean | मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
| searchByPages | Boolean | मान जो दर्शाता है कि क्या खोज पृष्ठों द्वारा की जाती है। |

### संबंधित देखें

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

डिफ़ॉल्ट मानों के साथ [`SearchOptions`](../../searchoptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। विवरण के लिए टिप्पणी देखें।

```csharp
public SearchOptions()
```

### टिप्पणियाँ

निम्नलिखित गुणों के डिफ़ॉल्ट मान हैं:

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### संबंधित देखें

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
