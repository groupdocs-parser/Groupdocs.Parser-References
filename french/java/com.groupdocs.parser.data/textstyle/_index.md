---
title: "TextStyle"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente le style du texte tel qu'un nom de police, une taille de police, etc."
type: docs
weight: 30
url: /fr/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Représente le style du texte tel qu'un nom de police, une taille de police, etc.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Initialise une nouvelle instance de la classe [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getName()](#getName--) | Obtient le nom du style. |
|
|  | [getFontName()](#getFontName--) | Obtient le nom de la police. |
|
|  | [getFontSize()](#getFontSize--) | Obtient la taille de la police. |
|
|  | [isBold()](#isBold--) | Obtient la valeur qui indique si la police est en gras. |
|
|  | [isItalic()](#isItalic--) | Obtient la valeur qui indique si la police est en italique. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Initialise une nouvelle instance de la classe [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | nom | java.lang.String | Le nom du style. |
|
|  | fontName | java.lang.String | Le nom de la police. |
|
|  | fontSize | double | La taille de la police. |
|
|  | bold | boolean | La valeur qui indique si la police est en gras. |
|
|  | italic | boolean | La valeur qui indique si la police est en italique. |
|

### getName() {#getName--}
```
public String getName()
```


Obtient le nom du style.


**Returns:**
java.lang.String - Une valeur chaîne qui représente le nom du style.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Obtient le nom de la police.


**Returns:**
java.lang.String - Une valeur chaîne qui représente le nom de la police.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Obtient la taille de la police.


**Returns:**
double - Une valeur double qui représente la taille de la police.

### isBold() {#isBold--}
```
public boolean isBold()
```


Obtient la valeur qui indique si la police est en gras.


**Returns:**
boolean -  true  si la police est en gras ; sinon,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtient la valeur qui indique si la police est en italique.


**Returns:**
boolean -  true  si la police est en italique ; sinon,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parameter | Type | Description |
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
