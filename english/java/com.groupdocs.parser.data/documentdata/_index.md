---
title: DocumentData
second_title: GroupDocs.Parser for Java API Reference
description: Represents data of the document.
type: docs
weight: 11
url: /java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object
```
public class DocumentData
```

Represents data of the document. It consists of [FieldData](../../com.groupdocs.parser.data/fielddata) objects which contain field data from document. An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class is used as return value of [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser\#parseByTemplate-Template-) and [Parser.parseForm()](../../com.groupdocs.parser/parser\#parseForm--) methods. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentData(Iterable<FieldData> fields)](#DocumentData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--) | Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the total number of the fields data. |
| [get(int index)](#get-int-) | Gets the field data by an index. |
| [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Returns the collection of field data where the name is equal to  fieldName . |
### DocumentData(Iterable<FieldData> fields) {#DocumentData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--}
```
public DocumentData(Iterable<FieldData> fields)
```


Initializes a new instance of the [FieldData](../../com.groupdocs.parser.data/fielddata) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fields | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | The collection of fields data. |

### getCount() {#getCount--}
```
public int getCount()
```


Gets the total number of the fields data.

**Returns:**
int - An integer value that represents the total number of the fields data.
### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Gets the field data by an index.

Iteration via all the fields:

```
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
```

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class. For example, [Parser.parseForm()](../../com.groupdocs.parser/parser\#parseForm--) method extracts only text fields:

```
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the field. |

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.
### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Returns the collection of field data where the name is equal to  fieldName .

Find fields by a field name:

```
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
```

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class. For example, [Parser.parseForm()](../../com.groupdocs.parser/parser\#parseForm--) method extracts only text fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | The name of the field. |

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - A collection of [FieldData](../../com.groupdocs.parser.data/fielddata) objects; empty collection if no field data is found.
