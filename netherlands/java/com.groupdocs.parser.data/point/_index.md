---
title: "Point"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een punt voor."
type: docs
weight: 25
url: /nl/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Stelt een punt voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Initialiseert een nieuwe instantie van de klasse [Point](../../com.groupdocs.parser.data/point). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getX()](#getX--) | Haalt de x-coördinaat op. |
|
|  | [getY()](#getY--) | Haalt de y-coördinaat op. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Converteert de tekenreeksrepresentatie van een punt naar de overeenkomstige klasse. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Initialiseert een nieuwe instantie van de klasse [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | x | double | De x-coördinaat. |
|
|  | y | double | De y-coördinaat. |
|

### getX() {#getX--}
```
public double getX()
```


Haalt de x-coördinaat op.


**Returns:**
double - Een double-waarde die de x-coördinaat weergeeft.

### getY() {#getY--}
```
public double getY()
```


Haalt de y-coördinaat op.


**Returns:**
double - Een double-waarde die de y-coördinaat weergeeft.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Converteert de tekenreeksrepresentatie van een punt naar de overeenkomstige klasse. Een retourwaarde geeft aan of de conversie geslaagd of mislukt is.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | s | java.lang.String | Een tekenreeks die een punt bevat om te converteren. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
