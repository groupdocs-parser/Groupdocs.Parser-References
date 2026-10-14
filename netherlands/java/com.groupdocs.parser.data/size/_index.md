---
title: "Size"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een grootte voor."
type: docs
weight: 28
url: /nl/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Stelt een grootte voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Initialiseert een nieuw exemplaar van de klasse [Size](../../com.groupdocs.parser.data/size). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getWidth()](#getWidth--) | Haalt de breedte op. |
|
|  | [getHeight()](#getHeight--) | Haalt de hoogte op. |
|
|  | [isEmpty()](#isEmpty--) | Haalt een waarde op die aangeeft of de grootte leeg is. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Converteert de tekenreeksrepresentatie van een grootte naar de overeenkomstige klasse. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Initialiseert een nieuw exemplaar van de klasse [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | breedte | double | De breedte in pixels. |
|
|  | hoogte | double | De hoogte in pixels. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Haalt de breedte op.


**Returns:**
double - Een double-waarde die de breedte in pixels vertegenwoordigt.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Haalt de hoogte op.


**Returns:**
double - Een double-waarde die de hoogte in pixels vertegenwoordigt.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Haalt een waarde op die aangeeft of de grootte leeg is.


**Returns:**
boolean -  true  als de  breedte  en  hoogte  nul zijn; anders,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Converteert de tekenreeksrepresentatie van een grootte naar de overeenkomstige klasse. Een retourwaarde geeft aan of de conversie geslaagd of mislukt is.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | s | java.lang.String | Een tekenreeks die een grootte bevat om te converteren. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
