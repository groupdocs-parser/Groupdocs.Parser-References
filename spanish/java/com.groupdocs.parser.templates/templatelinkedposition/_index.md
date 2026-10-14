---
title: "TemplateLinkedPosition"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona una posición de campo de plantilla que utiliza el campo vinculado."
type: docs
weight: 15
url: /es/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Proporciona una posición de campo de plantilla que utiliza el campo vinculado.

El siguiente ejemplo muestra el código para la situación si se sabe que el campo con un número de factura
se coloca a la derecha de la cadena "Invoice number" se usa el siguiente código:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Inicializa una nueva instancia de la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Inicializa una nueva instancia de la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) con nombre en MAYÚSCULAS. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Inicializa una nueva instancia de la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Obtiene el nombre del campo vinculado. |
|
|  | [getSearchArea()](#getSearchArea--) | Obtiene el tamaño del área donde se busca un campo. |
|
|  | [isAutoScale()](#isAutoScale--) | Obtiene el valor que indica si  SearchArea  se escala por el tamaño del campo vinculado. |
|
|  | [getEdges()](#getEdges--) | Obtiene los bordes del campo vinculado donde se busca un campo. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Inicializa una nueva instancia de la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | El nombre del campo vinculado. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | El tamaño del área donde se busca un campo. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Los bordes del campo vinculado donde se busca un campo. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Inicializa una nueva instancia de la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) con nombre en MAYÚSCULAS.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | El nombre del campo vinculado. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | El tamaño del área donde se busca un campo. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Los bordes del campo vinculado donde se busca un campo. |
|
|  | autoScale | boolean | El valor que indica si searchArea se escala por el tamaño del campo vinculado. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | El nombre del campo vinculado. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | El tamaño del área donde se busca un campo. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Los bordes del campo vinculado donde se busca un campo. |
|
|  | autoScale | boolean | El valor que indica si searchArea se escala por el tamaño del campo vinculado.\\ |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Obtiene el nombre del campo vinculado.


**Returns:**
java.lang.String - Un valor de cadena en mayúsculas que representa el nombre del campo vinculado.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Obtiene el tamaño del área donde se busca un campo.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Obtiene el valor que indica si  SearchArea  se escala por el tamaño del campo vinculado.


**Returns:**
java.lang.Boolean - {code true} si  SearchArea  se escala por el tamaño del campo vinculado; de lo contrario,  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Obtiene los bordes del campo vinculado donde se busca un campo.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crea una copia de la posición actual con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
