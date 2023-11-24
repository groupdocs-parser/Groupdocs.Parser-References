---
title: FieldData
second_title: GroupDocs.Parser for Java API Reference
description: Represents field data such as a name a page index a field value and so on.
type: docs
weight: 13
url: /java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Represents field data such as a name, a page index, a field value and so on. Depending on the field the value can be a text, an image, a table and so on.

The instances of [FieldData](../../com.groupdocs.parser.data/fielddata) class are used in [DocumentData](../../com.groupdocs.parser.data/documentdata) collection.
## Constructors

| Constructor | Description |
| --- | --- |
| [FieldData(String name, PageArea pageArea)](#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-) | Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class with UPPER CASE name. |
| [FieldData(String name, PageArea pageArea, boolean useUpperCaseName)](#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-boolean-) | Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class. |
| [FieldData(String name, PageArea pageArea, FieldData linkedField)](#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-com.groupdocs.parser.data.FieldData-) | Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class with UPPER CASE name. |
| [FieldData(String name, PageArea pageArea, FieldData linkedField, boolean useUpperCaseName)](#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-com.groupdocs.parser.data.FieldData-boolean-) | Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class. |
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--) | Gets the field name. |
| [getPageIndex()](#getPageIndex--) | Gets the page index. |
| [getPageArea()](#getPageArea--) | Gets the value of the field. |
| [getLinkedField()](#getLinkedField--) | Gets the linked field. |
| [getText()](#getText--) | Gets the text. |
| [getUseUpperCaseName()](#getUseUpperCaseName--) | Gets a value that indicates whether a  Name  was converted to UPPER CASE. |
### FieldData(String name, PageArea pageArea) {#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-}
```
public FieldData(String name, PageArea pageArea)
```


Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class with UPPER CASE name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the field. |
| pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | The value of the field. |

### FieldData(String name, PageArea pageArea, boolean useUpperCaseName) {#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-boolean-}
```
public FieldData(String name, PageArea pageArea, boolean useUpperCaseName)
```


Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the field. |
| pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | The value of the field. |
| useUpperCaseName | boolean | The value that indicates whether a  name  is converted to UPPER CASE. |

### FieldData(String name, PageArea pageArea, FieldData linkedField) {#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-com.groupdocs.parser.data.FieldData-}
```
public FieldData(String name, PageArea pageArea, FieldData linkedField)
```


Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class with UPPER CASE name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the field. |
| pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | The value of the field. |
| linkedField | [FieldData](../../com.groupdocs.parser.data/fielddata) | The field which is linked to the field. |

### FieldData(String name, PageArea pageArea, FieldData linkedField, boolean useUpperCaseName) {#FieldData-java.lang.String-com.groupdocs.parser.data.PageArea-com.groupdocs.parser.data.FieldData-boolean-}
```
public FieldData(String name, PageArea pageArea, FieldData linkedField, boolean useUpperCaseName)
```


Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the field. |
| pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | The value of the field. |
| linkedField | [FieldData](../../com.groupdocs.parser.data/fielddata) | The field which is linked to the field. |
| useUpperCaseName | boolean | The value that indicates whether a  name  is converted to UPPER CASE. |

### getName() {#getName--}
```
public String getName()
```


Gets the field name.

**Returns:**
java.lang.String - An uppercase string value that represents the name of the field.
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Gets the page index.

**Returns:**
int - A zero-based index of the page that contains the field.
### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Gets the value of the field.

Depending on field PageArea property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class. For example, [Parser.parseForm()](../../com.groupdocs.parser/parser\#parseForm--) method extracts only text fields.

```
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
```

**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.
### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Gets the linked field.

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.
### getText() {#getText--}
```
public String getText()
```


Gets the text.

**Returns:**
java.lang.String - A string value that represents a value of the field text;  null  if [PageArea](../../com.groupdocs.parser.data/pagearea) property isn't [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).
### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Gets a value that indicates whether a  Name  was converted to UPPER CASE.

**Returns:**
boolean - A boolean value that indicates whether a  Name  was converted to UPPER CASE.
