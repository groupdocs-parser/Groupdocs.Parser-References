---
title: "Point"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Punkt dar."
type: docs
weight: 25
url: /de/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Stellt einen Punkt dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Initialisiert eine neue Instanz der [Point](../../com.groupdocs.parser.data/point)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getX()](#getX--) | Liefert die x-Koordinate. |
|
|  | [getY()](#getY--) | Liefert die y-Koordinate. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Konvertiert die Zeichenkettenrepräsentation eines Punktes in das entsprechende Klassenobjekt. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Initialisiert eine neue Instanz der [Point](../../com.groupdocs.parser.data/point)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | x | double | Die x-Koordinate. |
|
|  | y | double | Die y-Koordinate. |
|

### getX() {#getX--}
```
public double getX()
```


Liefert die x-Koordinate.


**Returns:**
double - Ein double-Wert, der die x-Koordinate darstellt.

### getY() {#getY--}
```
public double getY()
```


Liefert die y-Koordinate.


**Returns:**
double - Ein double-Wert, der die y-Koordinate darstellt.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Konvertiert die Zeichenkettenrepräsentation eines Punktes in das entsprechende Klassenobjekt. Ein Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | s | java.lang.String | Eine Zeichenkette, die einen zu konvertierenden Punkt enthält. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
