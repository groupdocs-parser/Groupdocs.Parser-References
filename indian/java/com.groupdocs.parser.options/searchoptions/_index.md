---
title: "SearchOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेक्स्ट सर्च के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 35
url: /hi/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

टेक्स्ट सर्च के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

एक [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का उदाहरण [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) मेथड में पैरामीटर के रूप में उपयोग किया जाता है।
वहाँ उपयोग उदाहरण देखें।

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए हाइलाइट विकल्पों के साथ खोज करने के लिए उपयोग किया जाता है। |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए समान हाइलाइट विकल्पों के साथ खोज करने के लिए उपयोग किया जाता है। |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो हाइलाइट निष्कर्षण के बिना खोज करने के लिए उपयोग किया जाता है। |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो पृष्ठों द्वारा खोज करने और हाइलाइट निष्कर्षण के बिना उपयोग किया जाता है। |
|
|  | [SearchOptions()](#SearchOptions--) | डिफ़ॉल्ट मानों के साथ [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं। |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | वह मान प्राप्त करता है जो दर्शाता है कि नियमित अभिव्यक्ति उपयोग की गई है या नहीं। |
|
|  | [isSearchByPages()](#isSearchByPages--) | वह मान प्राप्त करता है जो दर्शाता है कि खोज पृष्ठों द्वारा की गई है या नहीं। |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | बाएँ हाइलाइट के विकल्प प्राप्त करता है। |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | दाएँ हाइलाइट के विकल्प प्राप्त करता है। |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | वह मान प्राप्त करता है जो खोज के लिए पृष्ठ के अधिकतम सूचकांक को दर्शाता है। |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | matchWholeWord | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है। |
|
|  | useRegularExpression | boolean | वह मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
|
|  | searchByPages | boolean | वह मान जो दर्शाता है कि क्या खोज पृष्ठों द्वारा की जाती है। |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | बाएँ हाइलाइट के विकल्प। |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | दाएँ हाइलाइट के विकल्प। |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | matchWholeWord | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है। |
|
|  | useRegularExpression | boolean | वह मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
|
|  | maxPageIndex | int | वह मान जो खोज के लिए पृष्ठ के अधिकतम अनुक्रमांक को दर्शाता है। |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | बाएँ हाइलाइट के विकल्प। |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | दाएँ हाइलाइट के विकल्प। |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए हाइलाइट विकल्पों के साथ खोज करने के लिए उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | matchWholeWord | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है। |
|
|  | useRegularExpression | boolean | वह मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | बाएँ हाइलाइट के विकल्प। |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | दाएँ हाइलाइट के विकल्प। |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो बाएँ और दाएँ हाइलाइट निष्कर्षण के लिए समान हाइलाइट विकल्पों के साथ खोज करने के लिए उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | matchWholeWord | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है। |
|
|  | useRegularExpression | boolean | वह मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | दोनों हाइलाइट्स के विकल्प। |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो हाइलाइट निष्कर्षण के बिना खोज करने के लिए उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | matchWholeWord | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है। |
|
|  | useRegularExpression | boolean | वह मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


नए [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है जो पृष्ठों द्वारा खोज करने और हाइलाइट निष्कर्षण के बिना उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | matchWholeWord | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है। |
|
|  | useRegularExpression | boolean | वह मान जो दर्शाता है कि क्या नियमित अभिव्यक्ति का उपयोग किया गया है। |
|
|  | searchByPages | boolean | वह मान जो दर्शाता है कि क्या खोज पृष्ठों द्वारा की जाती है। |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


डिफ़ॉल्ट मानों के साथ [SearchOptions](../../com.groupdocs.parser.options/searchoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। विवरण के लिए टिप्पणी देखें।

निम्नलिखित प्रॉपर्टीज़ के डिफ़ॉल्ट मान हैं:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है।


**Returns:**
boolean -  true  यदि टेक्स्ट केस को अनदेखा नहीं किया गया है; अन्यथा,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट खोज पूरे शब्द द्वारा सीमित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेक्स्ट खोज को पूरे शब्द तक सीमित किया गया है; अन्यथा,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


वह मान प्राप्त करता है जो दर्शाता है कि नियमित अभिव्यक्ति उपयोग की गई है या नहीं।


**Returns:**
बूलियन -  true  यदि नियमित अभिव्यक्ति का उपयोग किया गया है; अन्यथा,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


वह मान प्राप्त करता है जो दर्शाता है कि खोज पृष्ठों द्वारा की गई है या नहीं।


**Returns:**
बूलियन -  true  यदि खोज पृष्ठों द्वारा की जाती है; अन्यथा,  false  और खोज पूरे दस्तावेज़ पर की जाती है बिना [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) प्रॉपर्टी मान को [SearchResult](../../com.groupdocs.parser.data/searchresult) क्लास में शामिल किए।

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


बाएँ हाइलाइट के विकल्प प्राप्त करता है।


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


दाएँ हाइलाइट के विकल्प प्राप्त करता है।


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


वह मान प्राप्त करता है जो खोज के लिए पृष्ठ के अधिकतम सूचकांक को दर्शाता है।


**Returns:**
int - एक पूर्णांक मान जो खोज के लिए पृष्ठ के अधिकतम अनुक्रमांक को दर्शाता है; यदि सेट नहीं है तो -1;

