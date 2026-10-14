---
title: "Rectangle"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет прямоугольную область."
type: docs
weight: 26
url: /ru/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Представляет прямоугольную область.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Инициализирует новый экземпляр класса [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Инициализирует новый экземпляр класса [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getLeft()](#getLeft--) | Получает координату x левой грани прямоугольной области. |
|
|  | [getTop()](#getTop--) | Получает координату y верхней грани прямоугольной области. |
|
|  | [getRight()](#getRight--) | Получает координату x правой грани прямоугольной области. |
|
|  | [getBottom()](#getBottom--) | Получает координату y нижней грани прямоугольной области. |
|
|  | [getPosition()](#getPosition--) | Получает координаты верхнего левого угла прямоугольной области. |
|
|  | [getSize()](#getSize--) | Получает размер. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Инициализирует новый экземпляр класса [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | left | double | Координата x левой грани прямоугольной области. |
|
|  | top | double | Координата y верхней грани прямоугольной области. |
|
|  | право | double | Координата x правой грани прямоугольной области. |
|
|  | низ | double | Координата y нижней грани прямоугольной области. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Инициализирует новый экземпляр класса [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Координаты верхнего левого угла прямоугольной области. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Размер прямоугольной области. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Получает координату x левой грани прямоугольной области.


**Returns:**
double - Значение типа double, представляющее координату x левой грани прямоугольной области.

### getTop() {#getTop--}
```
public double getTop()
```


Получает координату y верхней грани прямоугольной области.


**Returns:**
double - Значение типа double, представляющее координату y верхней грани прямоугольной области.

### getRight() {#getRight--}
```
public double getRight()
```


Получает координату x правой грани прямоугольной области.


**Returns:**
double - Значение типа double, представляющее координату x правой грани прямоугольной области.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Получает координату y нижней грани прямоугольной области.


**Returns:**
double - Значение типа double, представляющее координату y нижней грани прямоугольной области.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Получает координаты верхнего левого угла прямоугольной области.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Получает размер.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
