---
title: "Rectangle"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une zone rectangulaire."
type: docs
weight: 26
url: /fr/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Représente une zone rectangulaire.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Initialise une nouvelle instance de la classe [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Initialise une nouvelle instance de la classe [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getLeft()](#getLeft--) | Obtient la coordonnée x du bord gauche de la zone rectangulaire. |
|
|  | [getTop()](#getTop--) | Obtient la coordonnée y du bord supérieur de la zone rectangulaire. |
|
|  | [getRight()](#getRight--) | Obtient la coordonnée x du bord droit de la zone rectangulaire. |
|
|  | [getBottom()](#getBottom--) | Obtient la coordonnée y du bord inférieur de la zone rectangulaire. |
|
|  | [getPosition()](#getPosition--) | Obtient les coordonnées du coin supérieur gauche de la zone rectangulaire. |
|
|  | [getSize()](#getSize--) | Obtient la taille. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Initialise une nouvelle instance de la classe [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | gauche | double | La coordonnée x du bord gauche de la zone rectangulaire. |
|
|  | haut | double | La coordonnée y du bord supérieur de la zone rectangulaire. |
|
|  | droite | double | La coordonnée x du bord droit de la zone rectangulaire. |
|
|  | bas | double | La coordonnée y du bord inférieur de la zone rectangulaire. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Initialise une nouvelle instance de la classe [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Les coordonnées du coin supérieur gauche de la zone rectangulaire. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | La taille de la zone rectangulaire. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Obtient la coordonnée x du bord gauche de la zone rectangulaire.


**Returns:**
double - Une valeur double qui représente la coordonnée x du bord gauche de la zone rectangulaire.

### getTop() {#getTop--}
```
public double getTop()
```


Obtient la coordonnée y du bord supérieur de la zone rectangulaire.


**Returns:**
double - Une valeur double qui représente la coordonnée y du bord supérieur de la zone rectangulaire.

### getRight() {#getRight--}
```
public double getRight()
```


Obtient la coordonnée x du bord droit de la zone rectangulaire.


**Returns:**
double - Une valeur double qui représente la coordonnée x du bord droit de la zone rectangulaire.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Obtient la coordonnée y du bord inférieur de la zone rectangulaire.


**Returns:**
double - Une valeur double qui représente la coordonnée y du bord inférieur de la zone rectangulaire.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Obtient les coordonnées du coin supérieur gauche de la zone rectangulaire.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Obtient la taille.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
