---
title: TemplateLinkedPosition
second_title: GroupDocs.Parser for Java API Reference
description: Provides a template field position which uses the linked field.
type: docs
weight: 15
url: /java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Provides a template field position which uses the linked field.

The following example shows the code for the situation if it's known that the field with an invoice number is placed on the right of "Invoice number" string the following code is used:

```
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
```
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Initializes a new instance of the [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class. |
| [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Initializes a new instance of the [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class with UPPER CASE name. |
| [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Initializes a new instance of the [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLinkedFieldName()](#getLinkedFieldName--) | Gets the linked field name. |
| [getSearchArea()](#getSearchArea--) | Gets the size of the area where a field is searched. |
| [isAutoScale()](#isAutoScale--) | Gets the value that indicates whether  SearchArea  is scaled by the linked field size. |
| [getEdges()](#getEdges--) | Gets the edges of the linked field where a field is searched. |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Initializes a new instance of the [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| linkedFieldName | java.lang.String | The name of the linked field. |
| searchArea | [Size](../../com.groupdocs.parser.data/size) | The size of the area where a field is searched. |
| edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | The edges of the linked field where a field is searched. |

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Initializes a new instance of the [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class with UPPER CASE name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| linkedFieldName | java.lang.String | The name of the linked field. |
| searchArea | [Size](../../com.groupdocs.parser.data/size) | The size of the area where a field is searched. |
| edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | The edges of the linked field where a field is searched. |
| autoScale | boolean | The value that indicates whether searchArea is scaled by the linked field size. |

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Initializes a new instance of the [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| linkedFieldName | java.lang.String | The name of the linked field. |
| searchArea | [Size](../../com.groupdocs.parser.data/size) | The size of the area where a field is searched. |
| edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | The edges of the linked field where a field is searched. |
| autoScale | boolean | The value that indicates whether searchArea is scaled by the linked field size.\\ |
| useUpperCaseName | boolean | The value that indicates whether a  name  is converted to UPPER CASE. |

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Gets the linked field name.

**Returns:**
java.lang.String - An uppercase string value that represents the linked field name.
### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Gets the size of the area where a field is searched.

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.
### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Gets the value that indicates whether  SearchArea  is scaled by the linked field size.

**Returns:**
java.lang.Boolean - \{code true\} if  SearchArea  is scaled by the linked field size; otherwise,  false .
### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Gets the edges of the linked field where a field is searched.

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.
