---
title: "PageTableArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет область таблицы на странице, которая используется для представления таблицы в функции разбора по шаблону."
type: docs
weight: 22
url: /ru/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Представляет область таблицы на странице, которая используется для представления таблицы в функции разбора по шаблону.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getCells()](#getCells--) | Получает коллекцию ячеек. |
|
|  | [getRowCount()](#getRowCount--) | Получает общее количество строк таблицы. |
|
|  | [getColumnCount()](#getColumnCount--) | Получает общее количество столбцов таблицы. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Возвращает высоту строки. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Возвращает ширину столбца. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Получает ячейку таблицы по индексам строки и столбца. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Примечание: проект C# помечает этот конструктор как
internal
(commit 954951f). В Java "internal-to-the-assembly"
не переводится чисто в package-private, потому что производители (
WordProcessingParser
,
TableAreaParser
,
и др.) находятся в
com.groupdocs.parser
, а не
com.groupdocs.parser.data
. Поэтому конструктор оставлен

public
чтобы кросс-пакетное создание всё ещё работало.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rows | java.lang.Iterable<java.lang.Double> | Коллекция высот строк. |
|
|  | columns | java.lang.Iterable<java.lang.Double> | Коллекция ширин столбцов. |
|
|  | cells | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | Коллекция ячеек. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая таблицу. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая таблицу. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Получает коллекцию ячеек. Обычная только для чтения коллекция ячеек таблицы.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Коллекция ячеек таблицы

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Получает общее количество строк таблицы.


**Returns:**
int - Целочисленное значение, содержащее общее количество строк таблицы.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Получает общее количество столбцов таблицы.


**Returns:**
int - Целочисленное значение, содержащее общее количество столбцов таблицы.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Возвращает высоту строки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rowIndex | int | Индекс строки, начинающийся с нуля. |
|

**Returns:**
double - Значение double, представляющее высоту строки.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Возвращает ширину столбца.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | columnIndex | int | Индекс столбца, начинающийся с нуля. |
|

**Returns:**
double - Значение типа double, представляющее ширину столбца.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Получает ячейку таблицы по индексам строки и столбца.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rowIndex | int | Нулевой индекс строки ячейки. |
|
|  | columnIndex | int | Нулевой индекс столбца ячейки. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

