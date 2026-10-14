---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет поле штрихкода шаблона."
type: docs
weight: 11
url: /ru/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Предоставляет поле штрихкода шаблона.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) с именем в верхнем регистре. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) с именем в верхнем регистре. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Получает прямоугольную область, содержащую поле штрихкода шаблона. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая поле штрихкода шаблона. |
|
|  | имя | java.lang.String | Имя поля штрихкода. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) с именем в верхнем регистре.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая поле штрихкода шаблона. |
|
|  | имя | java.lang.String | Имя поля штрихкода. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) с именем в верхнем регистре.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая поле штрихкода шаблона. |
|
|  | имя | java.lang.String | Имя поля штрихкода. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая поле штрихкода шаблона. |
|
|  | имя | java.lang.String | Имя поля штрихкода. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая поле штрихкода шаблона. |
|
|  | имя | java.lang.String | Имя поля штрихкода. |
|
|  | pageIndex | java.lang.Integer | Целочисленное значение, представляющее индекс страницы, на которой находится элемент шаблона; null, если элемент шаблона находится на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Получает прямоугольную область, содержащую поле штрихкода шаблона.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

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
