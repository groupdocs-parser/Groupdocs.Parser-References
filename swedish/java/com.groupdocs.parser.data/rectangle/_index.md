---
title: "Rectangle"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett rektangulärt område."
type: docs
weight: 26
url: /sv/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Representerar ett rektangulärt område.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Initierar en ny instans av klassen [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Initierar en ny instans av klassen [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getLeft()](#getLeft--) | Hämtar x-koordinaten för den vänstra kanten av det rektangulära området. |
|
|  | [getTop()](#getTop--) | Hämtar y-koordinaten för den övre kanten av det rektangulära området. |
|
|  | [getRight()](#getRight--) | Hämtar x-koordinaten för den högra kanten av det rektangulära området. |
|
|  | [getBottom()](#getBottom--) | Hämtar y-koordinaten för den nedre kanten av det rektangulära området. |
|
|  | [getPosition()](#getPosition--) | Hämtar koordinaterna för det övre vänstra hörnet av det rektangulära området. |
|
|  | [getSize()](#getSize--) | Hämtar storleken. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Initierar en ny instans av klassen [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | vänster | double | x-koordinaten för den vänstra kanten av det rektangulära området. |
|
|  | övre | double | y-koordinaten för den övre kanten av det rektangulära området. |
|
|  | höger | double | x-koordinaten för den högra kanten av det rektangulära området. |
|
|  | botten | double | y-koordinaten för den nedre kanten av det rektangulära området. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Initierar en ny instans av klassen [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Koordinaterna för det övre vänstra hörnet av det rektangulära området. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Storleken på det rektangulära området. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Hämtar x-koordinaten för den vänstra kanten av det rektangulära området.


**Returns:**
double - Ett dubbelvärde som representerar x-koordinaten för den vänstra kanten av det rektangulära området.

### getTop() {#getTop--}
```
public double getTop()
```


Hämtar y-koordinaten för den övre kanten av det rektangulära området.


**Returns:**
double - Ett dubbelvärde som representerar y-koordinaten för den övre kanten av det rektangulära området.

### getRight() {#getRight--}
```
public double getRight()
```


Hämtar x-koordinaten för den högra kanten av det rektangulära området.


**Returns:**
double - Ett dubbelvärde som representerar x-koordinaten för den högra kanten av det rektangulära området.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Hämtar y-koordinaten för den nedre kanten av det rektangulära området.


**Returns:**
double - Ett dubbelvärde som representerar y-koordinaten för den nedre kanten av det rektangulära området.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Hämtar koordinaterna för det övre vänstra hörnet av det rektangulära området.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Hämtar storleken.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
