---
title: "Size"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en storlek."
type: docs
weight: 28
url: /sv/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Representerar en storlek.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Initierar en ny instans av klassen [Size](../../com.groupdocs.parser.data/size). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getWidth()](#getWidth--) | Hämtar bredden. |
|
|  | [getHeight()](#getHeight--) | Hämtar höjden. |
|
|  | [isEmpty()](#isEmpty--) | Hämtar ett värde som indikerar om storleken är tom. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Konverterar strängrepresentationen av en storlek till dess motsvarande klass. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Initierar en ny instans av klassen [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | bredd | double | Bredden i pixlar. |
|
|  | höjd | double | Höjden i pixlar. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Hämtar bredden.


**Returns:**
double - Ett double‑värde som representerar bredden i pixlar.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Hämtar höjden.


**Returns:**
double - Ett double‑värde som representerar höjden i pixlar.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Hämtar ett värde som indikerar om storleken är tom.


**Returns:**
boolean -  true  om bredden och höjden är noll; annars,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Konverterar strängrepresentationen av en storlek till dess motsvarande klass. Ett returvärde indikerar om konverteringen lyckades eller misslyckades.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | s | java.lang.String | En sträng som innehåller en storlek att konvertera. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
