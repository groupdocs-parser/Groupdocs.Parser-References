---
title: TemplateBarcode
second_title: GroupDocs.Parser for Java API Reference
description: Provides the template barcode field.
type: docs
weight: 11
url: /java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Provides the template barcode field.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Initializes a new instance of the [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) class. |
| [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Initializes a new instance of the [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas with the UPPER CASE name. |
| [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Initializes a new instance of the [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that contains the template barcode field. |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Initializes a new instance of the [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the template barcode field. |
| name | java.lang.String | The barcode field name. |

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Initializes a new instance of the [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas with the UPPER CASE name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the template barcode field. |
| name | java.lang.String | The barcode field name. |
| pageIndex | java.lang.Integer | An integer value that represents the index of the page where the template item is located;  null  if the template item is located on any page. |

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initializes a new instance of the [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the template barcode field. |
| name | java.lang.String | The barcode field name. |
| pageIndex | java.lang.Integer | An integer value that represents the index of the page where the template item is located;  null  if the template item is located on any page. |
| useUpperCaseName | boolean | The value that indicates whether a  name  is converted to UPPER CASE. |

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that contains the template barcode field.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.
