---
title: "Point"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en punkt."
type: docs
weight: 25
url: /sv/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Representerar en punkt.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Initierar en ny instans av klassen [Point](../../com.groupdocs.parser.data/point). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getX()](#getX--) | Hämtar x-koordinaten. |
|
|  | [getY()](#getY--) | Hämtar y-koordinaten. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Konverterar strängrepresentationen av en punkt till dess klassmotsvarighet. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Initierar en ny instans av klassen [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | x | double | X-koordinaten. |
|
|  | y | double | Y-koordinaten. |
|

### getX() {#getX--}
```
public double getX()
```


Hämtar x-koordinaten.


**Returns:**
double - Ett double‑värde som representerar x-koordinaten.

### getY() {#getY--}
```
public double getY()
```


Hämtar y-koordinaten.


**Returns:**
double - Ett double‑värde som representerar y-koordinaten.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Konverterar strängrepresentationen av en punkt till dess klassmotsvarighet. Ett returvärde indikerar om konverteringen lyckades eller misslyckades.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | s | java.lang.String | En sträng som innehåller en punkt att konvertera. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
