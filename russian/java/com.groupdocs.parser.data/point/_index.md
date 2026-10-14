---
title: "Point"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет точку."
type: docs
weight: 25
url: /ru/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Представляет точку.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Инициализирует новый экземпляр класса [Point](../../com.groupdocs.parser.data/point). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getX()](#getX--) | Получает координату x. |
|
|  | [getY()](#getY--) | Получает координату y. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Преобразует строковое представление точки в эквивалентный объект класса. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Инициализирует новый экземпляр класса [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | x | double | Координата x. |
|
|  | y | double | Координата y. |
|

### getX() {#getX--}
```
public double getX()
```


Получает координату x.


**Returns:**
double - Дробное значение, представляющее координату x.

### getY() {#getY--}
```
public double getY()
```


Получает координату y.


**Returns:**
double - Дробное значение, представляющее координату y.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Преобразует строковое представление точки в её эквивалент класса. Возвращаемое значение указывает, успешно ли выполнено преобразование или нет.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | s | java.lang.String | Строка, содержащая точку для преобразования. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
