---
title: SearchResult
second_title: GroupDocs.Parser for Java API Reference
description: Represents the search result in the search functionality.
type: docs
weight: 27
url: /java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Represents the search result in the search functionality.

An instance of SearchResult class is used as return value of [Parser.search(String)](../../com.groupdocs.parser/parser\#search-String-) and [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser\#search-String--com.groupdocs.parser.options.SearchOptions-) methods. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Initializes a new instance of the [SearchResult](../../com.groupdocs.parser.data/searchresult) class. |
| [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Initializes a new instance of the [SearchResult](../../com.groupdocs.parser.data/searchresult) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPosition()](#getPosition--) | Gets the position in the document text. |
| [getText()](#getText--) | Gets the text. |
| [getPageIndex()](#getPageIndex--) | Gets the page index where the text is found. |
| [getLeftHighlightItem()](#getLeftHighlightItem--) | Gets the left highlight. |
| [getRightHighlightItem()](#getRightHighlightItem--) | Gets the right highlight. |
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Initializes a new instance of the [SearchResult](../../com.groupdocs.parser.data/searchresult) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | int | The position in the document text. |
| text | java.lang.String | The found text. |
| pageIndex | java.lang.Integer | The page index where the text is found. |
| leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | The left highlight. |
| rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | The right highlight. |

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Initializes a new instance of the [SearchResult](../../com.groupdocs.parser.data/searchresult) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | int | The position in the document text. |
| text | java.lang.String | The found text. |
| pageIndex | java.lang.Integer | The page index where the text is found. |

### getPosition() {#getPosition--}
```
public int getPosition()
```


Gets the position in the document text.

**Returns:**
int - A zero-based index of the start position of the search result.
### getText() {#getText--}
```
public String getText()
```


Gets the text.

**Returns:**
java.lang.String - A string value that respresents the found text.
### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Gets the page index where the text is found.

**Returns:**
java.lang.Integer - A zero-based index of the page where the text is found;  null  if the seach is performed on the whole document text.
### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Gets the left highlight.

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.
### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Gets the right highlight.

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.
