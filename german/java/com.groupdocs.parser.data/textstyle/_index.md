---
title: "TextStyle"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt den Stil des Textes dar, wie z. B. einen Schriftartnamen, eine Schriftgröße usw."
type: docs
weight: 30
url: /de/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Stellt den Stil des Textes dar, wie einen Schriftartnamen, eine Schriftgröße und so weiter.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Initialisiert eine neue Instanz der [TextStyle](../../com.groupdocs.parser.data/textstyle)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getName()](#getName--) | Liefert den Stilnamen. |
|
|  | [getFontName()](#getFontName--) | Liefert den Schriftartnamen. |
|
|  | [getFontSize()](#getFontSize--) | Liefert die Schriftgröße. |
|
|  | [isBold()](#isBold--) | Liefert den Wert, der angibt, ob die Schrift fett ist. |
|
|  | [isItalic()](#isItalic--) | Liefert den Wert, der angibt, ob die Schrift kursiv ist. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Initialisiert eine neue Instanz der [TextStyle](../../com.groupdocs.parser.data/textstyle)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Name | java.lang.String | Der Name des Stils. |
|
|  | fontName | java.lang.String | Der Name der Schriftart. |
|
|  | fontSize | double | Die Größe der Schriftart. |
|
|  | bold | boolean | Der Wert, der angibt, ob die Schrift fett ist. |
|
|  | italic | boolean | Der Wert, der angibt, ob die Schrift kursiv ist. |
|

### getName() {#getName--}
```
public String getName()
```


Liefert den Stilnamen.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Stilnamen darstellt.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Liefert den Schriftartnamen.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Schriftartnamen darstellt.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Liefert die Schriftgröße.


**Returns:**
double - Ein double-Wert, der die Schriftgröße darstellt.

### isBold() {#isBold--}
```
public boolean isBold()
```


Liefert den Wert, der angibt, ob die Schrift fett ist.


**Returns:**
boolean -  true  wenn die Schrift fett ist; andernfalls,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Liefert den Wert, der angibt, ob die Schrift kursiv ist.


**Returns:**
boolean -  true  wenn die Schrift kursiv ist; andernfalls,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
