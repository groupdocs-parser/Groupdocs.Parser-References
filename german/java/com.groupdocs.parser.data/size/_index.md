---
title: "Size"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Größe dar."
type: docs
weight: 28
url: /de/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Stellt eine Größe dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Initialisiert eine neue Instanz der [Size](../../com.groupdocs.parser.data/size)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getWidth()](#getWidth--) | Liefert die Breite. |
|
|  | [getHeight()](#getHeight--) | Liefert die Höhe. |
|
|  | [isEmpty()](#isEmpty--) | Liefert einen Wert, der angibt, ob die Größe leer ist. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Konvertiert die String-Darstellung einer Größe in das entsprechende Klassenobjekt. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Initialisiert eine neue Instanz der [Size](../../com.groupdocs.parser.data/size)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Breite | double | Die Breite in Pixeln. |
|
|  | Höhe | double | Die Höhe in Pixeln. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Liefert die Breite.


**Returns:**
double - Ein double-Wert, der die Breite in Pixeln darstellt.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Liefert die Höhe.


**Returns:**
double - Ein double-Wert, der die Höhe in Pixeln darstellt.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Liefert einen Wert, der angibt, ob die Größe leer ist.


**Returns:**
boolean -  true  wenn die  Breite  und  Höhe  null sind; andernfalls,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Konvertiert die String-Darstellung einer Größe in das entsprechende Klassenobjekt. Ein Rückgabewert gibt an, ob die Konvertierung erfolgreich war oder fehlgeschlagen ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | s | java.lang.String | Ein String, der eine zu konvertierende Größe enthält. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
