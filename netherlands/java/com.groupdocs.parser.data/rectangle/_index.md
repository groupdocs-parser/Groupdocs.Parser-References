---
title: "Rechthoek"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een rechthoekig gebied voor."
type: docs
weight: 26
url: /nl/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Stelt een rechthoekig gebied voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Initialiseert een nieuw exemplaar van de klasse [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Initialiseert een nieuw exemplaar van de klasse [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getLeft()](#getLeft--) | Haalt de x-coördinaat op van de linkerrand van het rechthoekige gebied. |
|
|  | [getTop()](#getTop--) | Haalt de y-coördinaat op van de bovenzijde van het rechthoekige gebied. |
|
|  | [getRight()](#getRight--) | Haalt de x-coördinaat op van de rechterrand van het rechthoekige gebied. |
|
|  | [getBottom()](#getBottom--) | Haalt de y-coördinaat op van de onderrand van het rechthoekige gebied. |
|
|  | [getPosition()](#getPosition--) | Haalt de coördinaten op van de linkerbovenhoek van het rechthoekige gebied. |
|
|  | [getSize()](#getSize--) | Haalt de grootte op. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Initialiseert een nieuw exemplaar van de klasse [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | left | double | De x-coördinaat van de linkerrand van het rechthoekige gebied. |
|
|  | top | double | De y-coördinaat van de bovenzijde van het rechthoekige gebied. |
|
|  | rechts | double | De x-coördinaat van de rechterrand van het rechthoekige gebied. |
|
|  | onder | double | De y-coördinaat van de onderrand van het rechthoekige gebied. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Initialiseert een nieuw exemplaar van de klasse [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | De coördinaten van de linkerbovenhoek van het rechthoekige gebied. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | De grootte van het rechthoekige gebied. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Haalt de x-coördinaat op van de linkerrand van het rechthoekige gebied.


**Returns:**
double - Een double-waarde die de x-coördinaat van de linkerrand van het rechthoekige gebied vertegenwoordigt.

### getTop() {#getTop--}
```
public double getTop()
```


Haalt de y-coördinaat op van de bovenzijde van het rechthoekige gebied.


**Returns:**
double - Een double-waarde die de y-coördinaat van de bovenzijde van het rechthoekige gebied vertegenwoordigt.

### getRight() {#getRight--}
```
public double getRight()
```


Haalt de x-coördinaat op van de rechterrand van het rechthoekige gebied.


**Returns:**
double - Een double-waarde die de x-coördinaat van de rechterrand van het rechthoekige gebied vertegenwoordigt.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Haalt de y-coördinaat op van de onderrand van het rechthoekige gebied.


**Returns:**
double - Een double-waarde die de y-coördinaat van de onderrand van het rechthoekige gebied vertegenwoordigt.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Haalt de coördinaten op van de linkerbovenhoek van het rechthoekige gebied.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Haalt de grootte op.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
