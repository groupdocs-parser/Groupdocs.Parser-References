---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет макет шаблонной таблицы, который используется классом для определения позиции таблицы."
type: docs
weight: 21
url: /ru/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Предоставляет макет шаблонной таблицы, который используется классом [TemplateTable](../../com.groupdocs.parser.templates/templatetable) для определения позиции таблицы.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Инициализирует новый экземпляр класса [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Получает прямоугольную область, содержащую таблицу. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Получает разделители столбцов таблицы. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Получает разделители строк таблицы. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Создаёт новый макет с тем же размером, разделителями и позицией в точке. |
|
|  | [scale(double factor)](#scale-double-) | Создаёт копию этого макета со всеми координатами, масштабированными на заданный коэффициент. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Инициализирует новый экземпляр класса [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Разделители столбцов таблицы. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Разделители строк таблицы. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Получает прямоугольную область, содержащую таблицу.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Получает разделители столбцов таблицы.


**Returns:**
java.util.List<java.lang.Double> - Коллекция значений double, представляющих x-координаты разделителей столбцов таблицы.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Получает разделители строк таблицы.


**Returns:**
java.util.List<java.lang.Double> - Коллекция значений double, представляющих y-координаты разделителей строк таблицы.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Создаёт новый макет с тем же размером, разделителями и позицией в точке.

Эта функция позволяет перемещать Table Layout.

Например, документ содержит таблицы на каждой странице (или набор документов с таблицей на странице).
Эти таблицы различаются по позиции и содержимому, но имеют одинаковые столбцы и строки. В этом случае пользователь
может определить объект [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) в точке (0, 0) один раз, а затем переместить его в место конкретной таблицы.

Если позиция таблицы зависит от другого объекта на странице, пользователь может определить объект [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)
на основе шаблонного документа и затем переместить его в соответствии с привязочным объектом. Например, если это сводная таблица
и за ней следует детальная таблица (которая может содержать различное количество строк). В этом случае пользователь может определить
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
метод возвращает копию текущего объекта. Пользователь может передать любые координаты
(даже отрицательные — тогда макет будет перемещён влево/вверх).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | Позиция нового макета. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Создаёт копию этого макета со всеми координатами, масштабированными на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | коэффициент | double | Коэффициент масштабирования. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

