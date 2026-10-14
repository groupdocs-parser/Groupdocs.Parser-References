---
title: "PageTextArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет текстовую область страницы, которая используется для представления текстового значения в функции разбора по шаблону или разбора форм."
type: docs
weight: 24
url: /ru/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Представляет текстовую область страницы, которая используется для представления текстового значения в функции разбора по шаблону или разбора форм.

Экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) используется в качестве возвращаемого значения следующих методов:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Также экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) используется в качестве значения свойства [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Смотрите примеры использования там.

Текстовая область может быть одиночной или составной. В первом случае она содержит текст, ограниченный прямоугольной областью.
Во втором случае она содержит другие текстовые области; свойства текста и таблицы вычисляются дочерними текстовыми областями.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Инициализирует новый экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getText()](#getText--) | Возвращает текст. |
|
|  | [getBaseLine()](#getBaseLine--) | Получает базовую линию. |
|
|  | [getTextStyle()](#getTextStyle--) | Получает стиль текста, такой как размер шрифта, название шрифта и т.д. |
|
|  | [getAreas()](#getAreas--) | Получает коллекцию дочерних текстовых областей страницы. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | текст | java.lang.String | Значение текста. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая текстовую область. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая текстовую область. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | текст | java.lang.String | Значение текста. |
|
|  | baseLine | java.lang.Double | Базовая линия текста. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Стиль текста. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая текстовую область. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая текстовую область. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Инициализирует новый экземпляр класса [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Коллекция дочерних текстовых областей страницы. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая текстовую область. |
|

### getText() {#getText--}
```
public String getText()
```


Возвращает текст.


**Returns:**
java.lang.String - Строковое значение, представляющее значение текстовой области страницы.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Получает базовую линию.


**Returns:**
double - Значение типа double, представляющее базовую линию.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Получает стиль текста, такой как размер шрифта, название шрифта и т.д.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Получает коллекцию дочерних текстовых областей страницы.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Коллекция дочерних текстовых областей страницы; пустая, если у текстовой области нет дочерних элементов.

