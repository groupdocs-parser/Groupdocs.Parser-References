---
title: "TextStyle"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de stijl van de tekst voor, zoals een lettertype‑naam, een lettergrootte, enzovoort."
type: docs
weight: 30
url: /nl/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Stelt de stijl van de tekst voor, zoals een lettertype‑naam, een lettergrootte en dergelijke.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Initialiseert een nieuwe instantie van de [TextStyle](../../com.groupdocs.parser.data/textstyle) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getName()](#getName--) | Haalt de stijlnaam op. |
|
|  | [getFontName()](#getFontName--) | Haalt de lettertype‑naam op. |
|
|  | [getFontSize()](#getFontSize--) | Haalt de lettergrootte op. |
|
|  | [isBold()](#isBold--) | Haalt de waarde op die aangeeft of het lettertype vet is. |
|
|  | [isItalic()](#isItalic--) | Haalt de waarde op die aangeeft of het lettertype cursief is. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Initialiseert een nieuwe instantie van de [TextStyle](../../com.groupdocs.parser.data/textstyle) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | naam | java.lang.String | De naam van de stijl. |
|
|  | fontName | java.lang.String | De naam van het lettertype. |
|
|  | fontSize | double | De grootte van het lettertype. |
|
|  | bold | boolean | De waarde die aangeeft of het lettertype vet is. |
|
|  | italic | boolean | De waarde die aangeeft of het lettertype cursief is. |
|

### getName() {#getName--}
```
public String getName()
```


Haalt de stijlnaam op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de stijlnaam weergeeft.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Haalt de lettertype‑naam op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de lettertype‑naam weergeeft.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Haalt de lettergrootte op.


**Returns:**
double - Een double‑waarde die de lettergrootte weergeeft.

### isBold() {#isBold--}
```
public boolean isBold()
```


Haalt de waarde op die aangeeft of het lettertype vet is.


**Returns:**
boolean -  true  als het lettertype vet is; anders,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Haalt de waarde op die aangeeft of het lettertype cursief is.


**Returns:**
boolean -  true  als het lettertype cursief is; anders,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
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
