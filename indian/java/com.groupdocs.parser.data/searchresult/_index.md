---
title: "SearchResult"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "खोज कार्यक्षमता में खोज परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 27
url: /hi/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

खोज कार्यक्षमता में खोज परिणाम का प्रतिनिधित्व करता है।

SearchResult वर्ग का एक उदाहरण [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-) के रिटर्न वैल्यू के रूप में उपयोग किया जाता है।
और [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) मेथड्स। वहाँ उपयोग के उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | [SearchResult](../../com.groupdocs.parser.data/searchresult) वर्ग का नया उदाहरण प्रारंभ करता है। |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | [SearchResult](../../com.groupdocs.parser.data/searchresult) वर्ग का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getPosition()](#getPosition--) | दस्तावेज़ पाठ में स्थिति प्राप्त करता है। |
|
|  | [getText()](#getText--) | टेक्स्ट प्राप्त करता है। |
|
|  | [getPageIndex()](#getPageIndex--) | पाठ जहाँ पाया जाता है, उस पृष्ठ का सूचकांक प्राप्त करता है। |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | बाएँ हाइलाइट को प्राप्त करता है। |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | दाएँ हाइलाइट को प्राप्त करता है। |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


[SearchResult](../../com.groupdocs.parser.data/searchresult) वर्ग का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्थिति | int | दस्तावेज़ पाठ में स्थिति। |
|
|  | पाठ | java.lang.String | पाया गया पाठ। |
|
|  | pageIndex | java.lang.Integer | पाठ जहाँ पाया जाता है, उस पृष्ठ का सूचकांक। |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | बाएँ हाइलाइट। |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | दाएँ हाइलाइट। |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


[SearchResult](../../com.groupdocs.parser.data/searchresult) वर्ग का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्थिति | int | दस्तावेज़ पाठ में स्थिति। |
|
|  | पाठ | java.lang.String | पाया गया पाठ। |
|
|  | pageIndex | java.lang.Integer | पाठ जहाँ पाया जाता है, उस पृष्ठ का सूचकांक। |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


दस्तावेज़ पाठ में स्थिति प्राप्त करता है।


**Returns:**
int - खोज परिणाम की प्रारंभिक स्थिति का शून्य-आधारित सूचकांक।

### getText() {#getText--}
```
public String getText()
```


टेक्स्ट प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो पाए गए पाठ का प्रतिनिधित्व करता है।

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


पाठ जहाँ पाया जाता है, उस पृष्ठ का सूचकांक प्राप्त करता है।


**Returns:**
java.lang.Integer - वह पृष्ठ जहाँ पाठ पाया जाता है, उसका शून्य-आधारित सूचकांक; यदि खोज पूरे दस्तावेज़ पाठ पर की जाती है तो null।

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


बाएँ हाइलाइट को प्राप्त करता है।


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


दाएँ हाइलाइट को प्राप्त करता है।


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

