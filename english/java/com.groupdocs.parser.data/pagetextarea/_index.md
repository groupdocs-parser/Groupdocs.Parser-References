---
title: PageTextArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents a page text area which is used to represent a text value in the parsing by template or parsing form functionality.
type: docs
weight: 24
url: /java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Represents a page text area which is used to represent a text value in the parsing by template or parsing form functionality.

An instance of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class is used as return value of the following methods:

 *  [Parser.getTextAreas()](../../com.groupdocs.parser/parser\#getTextAreas--)
 *  [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser\#getTextAreas-PageTextAreaOptions-)
 *  [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser\#getTextAreas-int-)
 *  [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser\#getTextAreas-int--PageTextAreaOptions-)

Also an instance of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class is used as value of [PageArea](../../com.groupdocs.parser.data/pagearea) property.

\*

See the usage examples there.

The text area can be single or composite. In the first case it contains a text which is bounded by a rectangular area. In the second case it contains other text areas; text and table properties are calculated by child text areas.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class. |
| [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class. |
| [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Initializes a new instance of the [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class. |
## Methods

| Method | Description |
| --- | --- |
| [getText()](#getText--) | Gets the text. |
| [getBaseLine()](#getBaseLine--) | Gets the base line. |
| [getTextStyle()](#getTextStyle--) | Gets the text style such as font size, font name an so on. |
| [getAreas()](#getAreas--) | Gets the collection of child text page areas. |
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Initializes a new instance of the [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The value of the text. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the text area. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the text area. |

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Initializes a new instance of the [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The value of the text. |
| baseLine | java.lang.Double | The base line of the text. |
| textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | The style of the text. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the text area. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the text area. |

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Initializes a new instance of the [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | The collecton of child text page areas. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the text area. |

### getText() {#getText--}
```
public String getText()
```


Gets the text.

**Returns:**
java.lang.String - A string value that represents a value of the text page area.
### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Gets the base line.

**Returns:**
double - A double value that represents the base line.
### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Gets the text style such as font size, font name an so on.

**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.
### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Gets the collection of child text page areas.

**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - A collection of child text page areas; empty if the text page area hasn't children.
