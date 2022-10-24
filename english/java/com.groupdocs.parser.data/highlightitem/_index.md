---
title: HighlightItem
second_title: GroupDocs.Parser for Java API Reference
description: Represents a highlight a part of the text which is usually used to explain the context of the found text in the search functionality.
type: docs
weight: 13
url: /java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Represents a highlight, a part of the text which is usually used to explain the context of the found text in the search functionality.

An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class is used as return value of [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser\#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) method, [SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult\#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult\#getRightHighlightItem--) properties. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Initializes a new instance of the [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPosition()](#getPosition--) | Gets the position in the document text. |
| [getText()](#getText--) | Gets the text of the highlight. |
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Initializes a new instance of the [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | int | The position in the document text. |
| text | java.lang.String | The text of the highlight. |

### getPosition() {#getPosition--}
```
public int getPosition()
```


Gets the position in the document text.

**Returns:**
int - A zero-based index of the start position of the highlight.
### getText() {#getText--}
```
public String getText()
```


Gets the text of the highlight.

**Returns:**
java.lang.String - A string value that represents the text of the highlight.
