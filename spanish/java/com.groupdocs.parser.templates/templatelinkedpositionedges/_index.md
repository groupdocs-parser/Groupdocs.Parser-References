---
title: "TemplateLinkedPositionEdges"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona los bordes del campo vinculado donde se busca el campo de texto."
type: docs
weight: 16
url: /es/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Proporciona los bordes del campo vinculado donde se busca el campo de texto. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) se usa en la clase [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Inicializa una nueva instancia de la clase [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Obtiene el valor que indica si la instancia está vacía. |
|
|  | [isLeft()](#isLeft--) | Obtiene el valor que indica si un campo se busca por la izquierda del campo vinculado. |
|
|  | [isTop()](#isTop--) | Obtiene el valor que indica si un campo se busca por arriba del campo vinculado. |
|
|  | [isRight()](#isRight--) | Obtiene el valor que indica si un campo se busca por la derecha del campo vinculado. |
|
|  | [isBottom()](#isBottom--) | Obtiene el valor que indica si un campo se busca por abajo del campo vinculado. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Convierte la representación en cadena de los bordes a su equivalente de clase. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Inicializa una nueva instancia de la clase [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | izquierda | boolean | El valor que indica si un campo se busca por la izquierda del campo vinculado. |
|
|  | arriba | boolean | El valor que indica si un campo se busca por arriba del campo vinculado. |
|
|  | derecha | boolean | El valor que indica si un campo se busca por la derecha del campo vinculado. |
|
|  | inferior | boolean | El valor que indica si un campo se busca por la parte inferior del campo vinculado. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Obtiene el valor que indica si la instancia está vacía.


**Returns:**
boolean -  true  si la instancia está vacía (todos los campos son  false ); de lo contrario,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Obtiene el valor que indica si un campo se busca por la izquierda del campo vinculado.


**Returns:**
boolean -  true  si un campo se busca por la izquierda del campo vinculado; de lo contrario,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Obtiene el valor que indica si un campo se busca por arriba del campo vinculado.


**Returns:**
boolean -  true  si un campo se busca por la parte superior del campo vinculado; de lo contrario,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Obtiene el valor que indica si un campo se busca por la derecha del campo vinculado.


**Returns:**
boolean -  true  si un campo se busca por la derecha del campo vinculado; de lo contrario,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Obtiene el valor que indica si un campo se busca por abajo del campo vinculado.


**Returns:**
boolean -  true  si un campo se busca por la parte inferior del campo vinculado; de lo contrario,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Convierte la representación en cadena de los bordes a su equivalente de clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | s | java.lang.String | Una cadena que contiene bordes para convertir. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
