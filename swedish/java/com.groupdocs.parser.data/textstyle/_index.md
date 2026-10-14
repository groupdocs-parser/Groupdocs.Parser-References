---
title: "TextStyle"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar textens stil såsom ett typsnittsnamn, en typsnittsstorlek och så vidare."
type: docs
weight: 30
url: /sv/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Representerar textens stil såsom ett typsnittsnamn, en typsnittsstorlek och så vidare.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Initierar en ny instans av klassen [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getName()](#getName--) | Hämtar stilnamnet. |
|
|  | [getFontName()](#getFontName--) | Hämtar typsnittsnamnet. |
|
|  | [getFontSize()](#getFontSize--) | Hämtar typsnittsstorleken. |
|
|  | [isBold()](#isBold--) | Hämtar värdet som indikerar om typsnittet är fet. |
|
|  | [isItalic()](#isItalic--) | Hämtar värdet som indikerar om typsnittet är kursiv. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Initierar en ny instans av klassen [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | namn | java.lang.String | Namnet på stilen. |
|
|  | fontName | java.lang.String | Namnet på typsnittet. |
|
|  | fontSize | double | Typsnittsstorleken. |
|
|  | bold | boolean | Värdet som indikerar om typsnittet är fet. |
|
|  | italic | boolean | Värdet som indikerar om typsnittet är kursiv. |
|

### getName() {#getName--}
```
public String getName()
```


Hämtar stilnamnet.


**Returns:**
java.lang.String - En strängvärde som representerar stilnamnet.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Hämtar typsnittsnamnet.


**Returns:**
java.lang.String - En strängvärde som representerar typsnittets namn.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Hämtar typsnittsstorleken.


**Returns:**
double - Ett dubbelvärde som representerar typsnittsstorleken.

### isBold() {#isBold--}
```
public boolean isBold()
```


Hämtar värdet som indikerar om typsnittet är fet.


**Returns:**
boolean -  true  om typsnittet är fet; annars  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Hämtar värdet som indikerar om typsnittet är kursiv.


**Returns:**
boolean -  true  om typsnittet är kursiv; annars  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
