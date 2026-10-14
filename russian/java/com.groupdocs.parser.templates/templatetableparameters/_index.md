---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры для алгоритмов обнаружения таблиц."
type: docs
weight: 22
url: /ru/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Предоставляет параметры для алгоритмов обнаружения таблиц.

Существует два алгоритма обнаружения таблицы:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

В некоторых случаях, когда алгоритмы не могут обнаружить таблицу или делают это неточно, используется класс [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Инициализирует новый экземпляр класса [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Инициализирует новый экземпляр класса [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Получает прямоугольную область, содержащую таблицу. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Получает разделители столбцов таблицы. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Возвращает значение, указывающее, содержит ли таблица объединённые ячейки. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Возвращает минимальное количество строк таблицы. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Возвращает минимальное количество столбцов таблицы. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Возвращает минимальное расстояние между столбцами таблицы. |
|
|  | [scale(double factor)](#scale-double-) | Создаёт копию этих параметров, масштабируя все координаты на заданный коэффициент. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Инициализирует новый экземпляр класса [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая таблицу. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Разделители столбцов таблицы. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Инициализирует новый экземпляр класса [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая таблицу. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Разделители столбцов таблицы. |
|
|  | mergedCells | java.lang.Boolean | Значение, указывающее, содержит ли таблицу объединённые ячейки. |
|
|  | minRowCount | java.lang.Integer | Минимальное количество строк таблицы. |
|
|  | minColumnCount | java.lang.Integer | Минимальное количество столбцов таблицы. |
|
|  | minVerticalSpace | java.lang.Integer | Минимальное расстояние между столбцами таблицы. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Получает прямоугольную область, содержащую таблицу.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Получает разделители столбцов таблицы.


**Returns:**
java.util.List<java.lang.Double> - Коллекция значений double, представляющих x‑координаты разделителей столбцов таблицы;  null  если не установлено.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Возвращает значение, указывающее, содержит ли таблица объединённые ячейки.


**Returns:**
java.lang.Boolean -  true  если таблица содержит объединённые ячейки; иначе,  false .  null  если не установлено.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Возвращает минимальное количество строк таблицы.


**Returns:**
java.lang.Integer - Целочисленное значение, представляющее минимальное количество строк таблицы;  null  если не установлено.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Возвращает минимальное количество столбцов таблицы.


**Returns:**
java.lang.Integer - Целочисленное значение, представляющее минимальное количество столбцов таблицы;  null  если не установлено.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Возвращает минимальное расстояние между столбцами таблицы.


**Returns:**
java.lang.Integer - Целочисленное значение, представляющее минимальное расстояние между столбцами таблицы;  null  если не установлено.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Создаёт копию этих параметров, масштабируя все координаты на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | коэффициент | double | Коэффициент масштабирования. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

