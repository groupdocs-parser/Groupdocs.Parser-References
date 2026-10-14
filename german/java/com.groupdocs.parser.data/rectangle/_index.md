---
title: "Rectangle"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen rechteckigen Bereich dar."
type: docs
weight: 26
url: /de/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Stellt einen rechteckigen Bereich dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Initialisiert eine neue Instanz der [Rectangle](../../com.groupdocs.parser.data/rectangle) Klasse. |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Initialisiert eine neue Instanz der [Rectangle](../../com.groupdocs.parser.data/rectangle) Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getLeft()](#getLeft--) | Liefert die x‑Koordinate der linken Kante des rechteckigen Bereichs. |
|
|  | [getTop()](#getTop--) | Liefert die y‑Koordinate der oberen Kante des rechteckigen Bereichs. |
|
|  | [getRight()](#getRight--) | Liefert die x‑Koordinate der rechten Kante des rechteckigen Bereichs. |
|
|  | [getBottom()](#getBottom--) | Liefert die y‑Koordinate der unteren Kante des rechteckigen Bereichs. |
|
|  | [getPosition()](#getPosition--) | Liefert die Koordinaten der oberen linken Ecke des rechteckigen Bereichs. |
|
|  | [getSize()](#getSize--) | Liefert die Größe. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Initialisiert eine neue Instanz der [Rectangle](../../com.groupdocs.parser.data/rectangle) Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | links | double | Die x‑Koordinate der linken Kante des rechteckigen Bereichs. |
|
|  | oben | double | Die y‑Koordinate der oberen Kante des rechteckigen Bereichs. |
|
|  | rechts | double | Die x‑Koordinate der rechten Kante des rechteckigen Bereichs. |
|
|  | unten | double | Die y‑Koordinate der unteren Kante des rechteckigen Bereichs. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Initialisiert eine neue Instanz der [Rectangle](../../com.groupdocs.parser.data/rectangle) Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Die Koordinaten der oberen linken Ecke des rechteckigen Bereichs. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Die Größe des rechteckigen Bereichs. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Liefert die x‑Koordinate der linken Kante des rechteckigen Bereichs.


**Returns:**
double - Ein double-Wert, der die x‑Koordinate der linken Kante des rechteckigen Bereichs darstellt.

### getTop() {#getTop--}
```
public double getTop()
```


Liefert die y‑Koordinate der oberen Kante des rechteckigen Bereichs.


**Returns:**
double - Ein double-Wert, der die y‑Koordinate der oberen Kante des rechteckigen Bereichs darstellt.

### getRight() {#getRight--}
```
public double getRight()
```


Liefert die x‑Koordinate der rechten Kante des rechteckigen Bereichs.


**Returns:**
double - Ein double-Wert, der die x‑Koordinate der rechten Kante des rechteckigen Bereichs darstellt.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Liefert die y‑Koordinate der unteren Kante des rechteckigen Bereichs.


**Returns:**
double - Ein double-Wert, der die y‑Koordinate der unteren Kante des rechteckigen Bereichs darstellt.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Liefert die Koordinaten der oberen linken Ecke des rechteckigen Bereichs.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Liefert die Größe.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
