---
title: PageTextAreaOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for page text areas extraction.
type: docs
weight: 26
url: /java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Provides the options which are used for page text areas extraction.

An instance of [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class is used as parameter in [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser\#getTextAreas-PageTextAreaOptions-) and [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser\#getTextAreas-int--PageTextAreaOptions-) methods. See the usage examples there.

**Learn more:**

 *  [Extract text areas][]


[Extract text areas]: https://docs.groupdocs.com/display/parserjava/Extract+text+areas
## Constructors

| Constructor | Description |
| --- | --- |
| [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Initializes a new instance of the [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class with the regular expression. |
| [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class with the regular expression and rectangular area. |
| [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getExpression()](#getExpression--) | Gets the regular expression. |
| [isMatchCase()](#isMatchCase--) | Gets the value that indicates whether a text case isn't ignored. |
| [isUniteSegments()](#isUniteSegments--) | Gets the value that indicates whether segments are united. |
| [isIgnoreFormatting()](#isIgnoreFormatting--) | Gets the value that indicates whether text formatting is ignored. |
### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Initializes a new instance of the [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class with the regular expression. Other options are set by default (see remarks for details).

The following properties have default values:

 *  MatchCase:  false 
 *  UniteSegments:  false 
 *  IgnoreFormatting:  false 
 *  Rectangle:  null 

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| expression | java.lang.String | The regular expression. |

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Initializes a new instance of the [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class with the regular expression and rectangular area. Other options are set by default (see remarks for details).

The following properties have default values:

 *  MatchCase:  false 
 *  UniteSegments:  false 
 *  IgnoreFormatting:  false 

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| expression | java.lang.String | The regular expression. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains page areas. |

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Initializes a new instance of the [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| expression | java.lang.String | The regular expression. |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |
| uniteSegments | boolean | The value that indicates whether segments are united. |
| ignoreFormatting | boolean | The value that indicates whether text formatting is ignored. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains page areas. |

### getExpression() {#getExpression--}
```
public String getExpression()
```


Gets the regular expression.

**Returns:**
java.lang.String - A string that represents the regular expression.
### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Gets the value that indicates whether a text case isn't ignored.

**Returns:**
boolean -  true  if a text case isn't ignored; otherwise,  false .
### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Gets the value that indicates whether segments are united.

**Returns:**
boolean - \{code true\} if segments are united; otherwise, \{code false\}.
### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Gets the value that indicates whether text formatting is ignored.

**Returns:**
boolean -  true  if text formatting is ignored; otherwise,  false .
