---
title: SearchOptions
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: क एक नय उदहरण प्ररंभ करत हैSearchOptionsgroupdocs.parser.options/searchoptions वर्ग.
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

का एक नया उदाहरण प्रारंभ करता है[`SearchOptions`](../../searchoptions) वर्ग.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो इंगित करता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है या नहीं। |
| matchWholeWord | Boolean | वह मान जो इंगित करता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं। |
| useRegularExpression | Boolean | वह मान जो बताता है कि रेगुलर एक्सप्रेशन का उपयोग किया गया है या नहीं. |
| searchByPages | Boolean | वह मान जो इंगित करता है कि खोज पृष्ठों द्वारा की गई है या नहीं। |
| leftHighlightOptions | HighlightOptions | बाएं हाइलाइट के लिए विकल्प। |
| rightHighlightOptions | HighlightOptions | सही हाइलाइट के लिए विकल्प। |

### यह सभी देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* नाम स्थान [GroupDocs.Parser.Options](../../searchoptions)
* सभा [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

का एक नया उदाहरण प्रारंभ करता है[`SearchOptions`](../../searchoptions) वर्ग जिसका उपयोग बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए हाइलाइट विकल्पों के साथ search के लिए किया जाता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो इंगित करता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है या नहीं। |
| matchWholeWord | Boolean | वह मान जो इंगित करता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं। |
| useRegularExpression | Boolean | वह मान जो बताता है कि रेगुलर एक्सप्रेशन का उपयोग किया गया है या नहीं. |
| leftHighlightOptions | HighlightOptions | बाएं हाइलाइट के लिए विकल्प। |
| rightHighlightOptions | HighlightOptions | सही हाइलाइट के लिए विकल्प। |

### यह सभी देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* नाम स्थान [GroupDocs.Parser.Options](../../searchoptions)
* सभा [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

का एक नया उदाहरण प्रारंभ करता है[`SearchOptions`](../../searchoptions) वर्ग जिसका उपयोग बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए समान हाइलाइट विकल्पों के साथ search के लिए किया जाता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो इंगित करता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है या नहीं। |
| matchWholeWord | Boolean | वह मान जो इंगित करता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं। |
| useRegularExpression | Boolean | वह मान जो बताता है कि रेगुलर एक्सप्रेशन का उपयोग किया गया है या नहीं. |
| highlightOptions | HighlightOptions | दोनों हाइलाइट्स के लिए विकल्प। |

### यह सभी देखें

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* नाम स्थान [GroupDocs.Parser.Options](../../searchoptions)
* सभा [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`SearchOptions`](../../searchoptions) वर्ग जिसका उपयोग हाइलाइट निष्कर्षण के बिना खोजने के लिए किया जाता है।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो इंगित करता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है या नहीं। |
| matchWholeWord | Boolean | वह मान जो इंगित करता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं। |
| useRegularExpression | Boolean | वह मान जो बताता है कि रेगुलर एक्सप्रेशन का उपयोग किया गया है या नहीं. |

### यह सभी देखें

* class [SearchOptions](../../searchoptions)
* नाम स्थान [GroupDocs.Parser.Options](../../searchoptions)
* सभा [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`SearchOptions`](../../searchoptions)वर्ग जिसका उपयोग पृष्ठों द्वारा खोज करने के लिए किया जाता है और हाइलाइट निष्कर्षण के बिना।

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| matchCase | Boolean | वह मान जो इंगित करता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है या नहीं। |
| matchWholeWord | Boolean | वह मान जो इंगित करता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं। |
| useRegularExpression | Boolean | वह मान जो बताता है कि रेगुलर एक्सप्रेशन का उपयोग किया गया है या नहीं. |
| searchByPages | Boolean | वह मान जो इंगित करता है कि खोज पृष्ठों द्वारा की गई है या नहीं। |

### यह सभी देखें

* class [SearchOptions](../../searchoptions)
* नाम स्थान [GroupDocs.Parser.Options](../../searchoptions)
* सभा [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`SearchOptions`](../../searchoptions) वर्ग डिफ़ॉल्ट मान के साथ। विवरण के लिए टिप्पणी देखें.

```csharp
public SearchOptions()
```

### टिप्पणियों

निम्नलिखित गुणों में डिफ़ॉल्ट मान हैं:

**[`MatchCase`](../matchcase)**

`असत्य`

**[`MatchWholeWord`](../matchwholeword)**

`असत्य`

**[`UseRegularExpression`](../useregularexpression)**

`असत्य`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`व्यर्थ`

**[`RightHighlightOptions`](../righthighlightoptions)**

`व्यर्थ`

### यह सभी देखें

* class [SearchOptions](../../searchoptions)
* नाम स्थान [GroupDocs.Parser.Options](../../searchoptions)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
