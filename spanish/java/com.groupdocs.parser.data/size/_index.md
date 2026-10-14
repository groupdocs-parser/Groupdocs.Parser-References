---
title: "Size"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un tamaño."
type: docs
weight: 28
url: /es/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Representa un tamaño.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Inicializa una nueva instancia de la clase [Size](../../com.groupdocs.parser.data/size). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getWidth()](#getWidth--) | Obtiene el ancho. |
|
|  | [getHeight()](#getHeight--) | Obtiene la altura. |
|
|  | [isEmpty()](#isEmpty--) | Obtiene un valor que indica si el tamaño está vacío. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Convierte la representación en cadena de un tamaño a su equivalente de clase. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Inicializa una nueva instancia de la clase [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | ancho | double | El ancho en píxeles. |
|
|  | altura | double | La altura en píxeles. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtiene el ancho.


**Returns:**
double - Un valor double que representa el ancho en píxeles.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtiene la altura.


**Returns:**
double - Un valor double que representa la altura en píxeles.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Obtiene un valor que indica si el tamaño está vacío.


**Returns:**
boolean -  true  si el  ancho  y la  altura  son cero; de lo contrario,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Convierte la representación en cadena de un tamaño a su equivalente de clase. Un valor de retorno indica si la conversión tuvo éxito o falló.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | s | java.lang.String | Una cadena que contiene un tamaño para convertir. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
