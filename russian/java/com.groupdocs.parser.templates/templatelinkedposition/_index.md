---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет позицию поля шаблона, использующую связанное поле."
type: docs
weight: 15
url: /ru/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Предоставляет позицию поля шаблона, использующую связанное поле.

Следующий пример показывает код для ситуации, когда известно, что поле с номером счета
расположено справа от строки "Invoice number", используется следующий код:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Инициализирует новый экземпляр класса [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Инициализирует новый экземпляр класса [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) с именем в ВЕРХНЕМ РЕГИСТРЕ. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Инициализирует новый экземпляр класса [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Получает имя связанного поля. |
|
|  | [getSearchArea()](#getSearchArea--) | Получает размер области, в которой ищется поле. |
|
|  | [isAutoScale()](#isAutoScale--) | Получает значение, указывающее, масштабируется ли  SearchArea  по размеру связанного поля. |
|
|  | [getEdges()](#getEdges--) | Получает границы связанного поля, где ищется поле. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Инициализирует новый экземпляр класса [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Имя связанного поля. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Размер области, в которой ищется поле. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Границы связанного поля, где ищется поле. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Инициализирует новый экземпляр класса [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) с именем в ВЕРХНЕМ РЕГИСТРЕ.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Имя связанного поля. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Размер области, в которой ищется поле. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Границы связанного поля, где ищется поле. |
|
|  | autoScale | boolean | Значение, указывающее, масштабируется ли searchArea по размеру связанного поля. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Имя связанного поля. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Размер области, в которой ищется поле. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Границы связанного поля, где ищется поле. |
|
|  | autoScale | boolean | Значение, указывающее, масштабируется ли searchArea по размеру связанного поля.\\ |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Получает имя связанного поля.


**Returns:**
java.lang.String - Строковое значение в верхнем регистре, представляющее имя связанного поля.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Получает размер области, в которой ищется поле.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Получает значение, указывающее, масштабируется ли  SearchArea  по размеру связанного поля.


**Returns:**
java.lang.Boolean - {code true} если  SearchArea  масштабируется по размеру связанного поля; иначе false.

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Получает границы связанного поля, где ищется поле.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Создаёт копию текущей позиции со всеми координатами, масштабированными на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| коэффициент | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
