---
title: "Size"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une taille."
type: docs
weight: 28
url: /fr/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Représente une taille.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Initialise une nouvelle instance de la classe [Size](../../com.groupdocs.parser.data/size). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getWidth()](#getWidth--) | Obtient la largeur. |
|
|  | [getHeight()](#getHeight--) | Obtient la hauteur. |
|
|  | [isEmpty()](#isEmpty--) | Obtient une valeur qui indique si la taille est vide. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Convertit la représentation sous forme de chaîne d'une taille en son équivalent de classe. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Initialise une nouvelle instance de la classe [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | largeur | double | La largeur en pixels. |
|
|  | hauteur | double | La hauteur en pixels. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtient la largeur.


**Returns:**
double - Une valeur double qui représente la largeur en pixels.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtient la hauteur.


**Returns:**
double - Une valeur double qui représente la hauteur en pixels.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Obtient une valeur qui indique si la taille est vide.


**Returns:**
boolean -  true  si la  largeur  et  la hauteur  sont zéro ; sinon,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Convertit la représentation sous forme de chaîne d'une taille en son équivalent de classe. Une valeur de retour indique si la conversion a réussi ou échoué.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | s | java.lang.String | Une chaîne contenant une taille à convertir. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
