---
title: "TextStyle"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa el estilo del texto, como el nombre de la fuente, el tamaño de la fuente, etc."
type: docs
weight: 30
url: /es/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Representa el estilo del texto, como el nombre de la fuente, el tamaño de la fuente, etc.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Inicializa una nueva instancia de la clase [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getName()](#getName--) | Obtiene el nombre del estilo. |
|
|  | [getFontName()](#getFontName--) | Obtiene el nombre de la fuente. |
|
|  | [getFontSize()](#getFontSize--) | Obtiene el tamaño de la fuente. |
|
|  | [isBold()](#isBold--) | Obtiene el valor que indica si la fuente está en negrita. |
|
|  | [isItalic()](#isItalic--) | Obtiene el valor que indica si la fuente está en cursiva. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Inicializa una nueva instancia de la clase [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | nombre | java.lang.String | El nombre del estilo. |
|
|  | fontName | java.lang.String | El nombre de la fuente. |
|
|  | fontSize | double | El tamaño de la fuente. |
|
|  | bold | boolean | El valor que indica si la fuente está en negrita. |
|
|  | italic | boolean | El valor que indica si la fuente está en cursiva. |
|

### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del estilo.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre del estilo.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Obtiene el nombre de la fuente.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre de la fuente.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Obtiene el tamaño de la fuente.


**Returns:**
double - Un valor double que representa el tamaño de la fuente.

### isBold() {#isBold--}
```
public boolean isBold()
```


Obtiene el valor que indica si la fuente está en negrita.


**Returns:**
boolean -  true  si la fuente está en negrita; de lo contrario,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtiene el valor que indica si la fuente está en cursiva.


**Returns:**
boolean -  true  si la fuente está en cursiva; de lo contrario,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
