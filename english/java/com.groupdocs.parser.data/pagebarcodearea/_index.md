---
title: PageBarcodeArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents a page barcode area which is used to represent a barcode value in the parsing by template functionality.
type: docs
weight: 17
url: /java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Represents a page barcode area which is used to represent a barcode value in the parsing by template functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageBarcodeArea(String value, String codeTypeName, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) class. |
## Methods

| Method | Description |
| --- | --- |
| [getValue()](#getValue--) | Gets the barcode value. |
| [getCodeTypeName()](#getCodeTypeName--) | Gets the name of the barcode type. |
### PageBarcodeArea(String value, String codeTypeName, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, Page page, Rectangle rectangle)
```


Initializes a new instance of the [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value of the barcode. |
| codeTypeName | java.lang.String | The type name of the barcode. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the barcode area. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the barcode area. |

### getValue() {#getValue--}
```
public String getValue()
```


Gets the barcode value.

**Returns:**
java.lang.String - A string value that represents a value of the barcode page area.
### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Gets the name of the barcode type.

**Returns:**
java.lang.String - A string value than represents a type name of the barcode.
