---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет границы связанного поля, где ищется текстовое поле."
type: docs
weight: 16
url: /ru/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Предоставляет границы связанного поля, где ищется текстовое поле. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) используется в классе [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Инициализирует новый экземпляр класса [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Возвращает значение, указывающее, пустой ли экземпляр. |
|
|  | [isLeft()](#isLeft--) | Возвращает значение, указывающее, ищется ли поле слева от связанного поля. |
|
|  | [isTop()](#isTop--) | Возвращает значение, указывающее, ищется ли поле сверху от связанного поля. |
|
|  | [isRight()](#isRight--) | Возвращает значение, указывающее, ищется ли поле справа от связанного поля. |
|
|  | [isBottom()](#isBottom--) | Возвращает значение, указывающее, ищется ли поле снизу от связанного поля. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Преобразует строковое представление границ в эквивалентный объект класса. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Инициализирует новый экземпляр класса [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | left | boolean | Значение, указывающее, ищется ли поле слева от связанного поля. |
|
|  | top | boolean | Значение, указывающее, ищется ли поле сверху от связанного поля. |
|
|  | право | boolean | Значение, указывающее, ищется ли поле справа от связанного поля. |
|
|  | низ | boolean | Значение, указывающее, ищется ли поле снизу от связанного поля. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Возвращает значение, указывающее, пустой ли экземпляр.


**Returns:**
boolean -  true  если экземпляр пуст (все поля равны false); иначе, false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Возвращает значение, указывающее, ищется ли поле слева от связанного поля.


**Returns:**
boolean -  true  если поле ищется слева от связанного поля; иначе, false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Возвращает значение, указывающее, ищется ли поле сверху от связанного поля.


**Returns:**
boolean -  true  если поле ищется сверху от связанного поля; иначе, false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Возвращает значение, указывающее, ищется ли поле справа от связанного поля.


**Returns:**
boolean -  true  если поле ищется справа от связанного поля; иначе, false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Возвращает значение, указывающее, ищется ли поле снизу от связанного поля.


**Returns:**
boolean -  true  если поле ищется снизу от связанного поля; иначе, false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Преобразует строковое представление границ в эквивалентный объект класса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | s | java.lang.String | Строка, содержащая границы для преобразования. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
