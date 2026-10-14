---
title: "TemplateLinkedPosition"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر موضع حقل القالب الذي يستخدم الحقل المرتبط."
type: docs
weight: 15
url: /ar/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

يوفر موضع حقل القالب الذي يستخدم الحقل المرتبط.

المثال التالي يوضح الشيفرة للحالة إذا كان معروفًا أن الحقل الذي يحتوي على رقم الفاتورة
موضعًا على يمين السلسلة "Invoice number" يتم استخدام الشيفرة التالية:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | يُنشئ مثيلاً جديدًا للفئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | يُنشئ مثيلاً جديدًا للفئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) باسم UPPER CASE. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | يُنشئ مثيلاً جديدًا للفئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | يحصل على اسم الحقل المرتبط. |
|
|  | [getSearchArea()](#getSearchArea--) | يحصل على حجم المنطقة التي يتم فيها البحث عن الحقل. |
|
|  | [isAutoScale()](#isAutoScale--) | يحصل على القيمة التي تشير إلى ما إذا كان  SearchArea  يتم تحجيمه بحجم الحقل المرتبط. |
|
|  | [getEdges()](#getEdges--) | يحصل على حواف الحقل المرتبط حيث يتم البحث عن الحقل. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | اسم الحقل المرتبط. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | حجم المنطقة التي يتم البحث فيها عن الحقل. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | حدود الحقل المرتبط حيث يتم البحث عن الحقل. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) باسم UPPER CASE.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | اسم الحقل المرتبط. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | حجم المنطقة التي يتم البحث فيها عن الحقل. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | حدود الحقل المرتبط حيث يتم البحث عن الحقل. |
|
|  | autoScale | boolean | القيمة التي تشير إلى ما إذا كانت مساحة البحث تُقاس وفق حجم الحقل المرتبط. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | اسم الحقل المرتبط. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | حجم المنطقة التي يتم البحث فيها عن الحقل. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | حدود الحقل المرتبط حيث يتم البحث عن الحقل. |
|
|  | autoScale | boolean | القيمة التي تشير إلى ما إذا كانت مساحة البحث تُقاس وفق حجم الحقل المرتبط.\\ |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


يحصل على اسم الحقل المرتبط.


**Returns:**
java.lang.String - قيمة سلسلة أحرف كبيرة تمثل اسم الحقل المرتبط.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


يحصل على حجم المنطقة التي يتم فيها البحث عن الحقل.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


يحصل على القيمة التي تشير إلى ما إذا كان  SearchArea  يتم تحجيمه بحجم الحقل المرتبط.


**Returns:**
java.lang.Boolean - {code true} إذا كانت مساحة البحث مُقاسة وفق حجم الحقل المرتبط؛ وإلا، false.

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


يحصل على حواف الحقل المرتبط حيث يتم البحث عن الحقل.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


ينشئ نسخة من الموضع الحالي مع تعديل جميع الإحداثيات وفق العامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| العامل | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
