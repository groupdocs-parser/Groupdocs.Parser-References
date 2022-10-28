---
title: PageHyperlinkArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents a page area which is used to represent a hyperlink on the page.
type: docs
weight: 19
url: /java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Represents a page area which is used to represent a hyperlink on the page.

An instance of [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) class is used as return value of the following methods:

 *  [Parser.getHyperlinks()](../../com.groupdocs.parser/parser\#getHyperlinks--)
 *  [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser\#getHyperlinks-PageAreaOptions-)
 *  [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser\#getHyperlinks-int-)
 *  [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser\#getHyperlinks-int--PageAreaOptions-)

See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) class. |
## Methods

| Method | Description |
| --- | --- |
| [getText()](#getText--) | Gets the hyperlink text. |
| [getUrl()](#getUrl--) | Gets the hyperlink URL. |
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Initializes a new instance of the [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The hyperlink text. |
| url | java.lang.String | The hyperlink URL. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the hyperlink. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the hyperlink. |

### getText() {#getText--}
```
public String getText()
```


Gets the hyperlink text.

**Returns:**
java.lang.String - A string value that represents hyperlink text.
### getUrl() {#getUrl--}
```
public String getUrl()
```


Gets the hyperlink URL.

**Returns:**
java.lang.String - A string value that represents hyperlink URL.
