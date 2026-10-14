---
title: "Point"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente un point."
type: docs
weight: 25
url: /fr/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Représente un point.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Initialise une nouvelle instance de la classe [Point](../../com.groupdocs.parser.data/point). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getX()](#getX--) | Obtient la coordonnée x. |
|
|  | [getY()](#getY--) | Obtient la coordonnée y. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Convertit la représentation sous forme de chaîne d'un point en son équivalent de classe. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Initialise une nouvelle instance de la classe [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | x | double | La coordonnée x. |
|
|  | y | double | La coordonnée y. |
|

### getX() {#getX--}
```
public double getX()
```


Obtient la coordonnée x.


**Returns:**
double - Une valeur double qui représente la coordonnée x.

### getY() {#getY--}
```
public double getY()
```


Obtient la coordonnée y.


**Returns:**
double - Une valeur double qui représente la coordonnée y.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Convertit la représentation sous forme de chaîne d'un point en son équivalent de classe. Une valeur de retour indique si la conversion a réussi ou échoué.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | s | java.lang.String | Une chaîne contenant un point à convertir. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
