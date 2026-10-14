---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения областей страниц."
type: docs
weight: 28
url: /ru/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Предоставляет параметры, используемые для извлечения областей страниц.

Экземпляр класса [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) используется в качестве параметра в методе [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
и методах [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). См. примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) с размером игнорируемой границы. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Инициализирует новый экземпляр класса [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Получает прямоугольную область, содержащую области страниц. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Получает размер границы, игнорируемой при захвате прямоугольной областью. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) с размером игнорируемой границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая области страниц. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Инициализирует новый экземпляр класса [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая области страниц. |
|
|  | rectangleTolerance | double | Размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Получает прямоугольную область, содержащую области страниц.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Получает размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента.


**Returns:**
double - Значение типа double от 0 (без границы) до 1 (игнорировать весь элемент).

