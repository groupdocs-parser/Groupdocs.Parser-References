---
title: TemplateItem
second_title: GroupDocs.Parser for Java API Reference
description: Provides a base abstract class for template items.
type: docs
weight: 14
url: /java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Provides a base abstract class for template items.

The inheritors of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class are used in [Template](../../com.groupdocs.parser.templates/template) collection.
## Methods

| Method | Description |
| --- | --- |
| [scale(double factor)](#scale-double-) | Creates a copy of the current item with all coordinates scaled by the given factor. |
| [getName()](#getName--) | Gets the name of the template item. |
| [getPageIndex()](#getPageIndex--) | Gets the page index of the template item. |
| [getPageWidth()](#getPageWidth--) | Gets the width of the page that was used to create the template item. |
| [getUseUpperCaseName()](#getUseUpperCaseName--) | Gets a value that indicates whether a  Name  was converted to UPPER CASE. |
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Creates a copy of the current item with all coordinates scaled by the given factor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| factor | double | The scaling factor. |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.
### getName() {#getName--}
```
public String getName()
```


Gets the name of the template item.

**Returns:**
java.lang.String - An uppercase string value that represents a name of the template item.
### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Gets the page index of the template item.

**Returns:**
java.lang.Integer - An integer value that represents the index of the page where the template item is located;  null  if the template item is located on any page.
### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Gets the width of the page that was used to create the template item.

**Returns:**
java.lang.Double - The width of the page in pixels;  null  if the page width is unknown.
### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Gets a value that indicates whether a  Name  was converted to UPPER CASE.

**Returns:**
boolean - A boolean value that indicates whether a  Name  was converted to UPPER CASE.
