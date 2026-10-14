---
title: "TemplateField"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет текстовое поле шаблона."
type: docs
weight: 12
url: /ru/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Предоставляет текстовое поле шаблона.

Текстовые поля определяются их позицией на странице. Существует три способа определить текстовое поле:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser/templates/templatefield) с именем в ВЕРХНЕМ РЕГИСТРЕ. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser/templates/templatefield) с именем в ВЕРХНЕМ РЕГИСТРЕ. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getPosition()](#getPosition--) | Получает значение, описывающее, как найти шаблонное поле на странице документа. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Позиция поля. |
|
|  | имя | java.lang.String | Имя поля. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser/templates/templatefield) с именем в ВЕРХНЕМ РЕГИСТРЕ.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Позиция поля. |
|
|  | имя | java.lang.String | Имя поля. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser/templates/templatefield) с именем в ВЕРХНЕМ РЕГИСТРЕ.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Позиция поля. |
|
|  | имя | java.lang.String | Имя поля. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Позиция поля. |
|
|  | имя | java.lang.String | Имя поля. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Позиция поля. |
|
|  | имя | java.lang.String | Имя поля. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Получает значение, описывающее, как найти шаблонное поле на странице документа.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Создаёт копию текущего элемента, масштабируя все координаты на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| коэффициент | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
