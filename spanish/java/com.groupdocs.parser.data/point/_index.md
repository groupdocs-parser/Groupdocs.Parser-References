---
title: "Point"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un punto."
type: docs
weight: 25
url: /es/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Representa un punto.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Inicializa una nueva instancia de la clase [Point](../../com.groupdocs.parser.data/point). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getX()](#getX--) | Obtiene la coordenada x. |
|
|  | [getY()](#getY--) | Obtiene la coordenada y. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Convierte la representación en cadena de un punto a su equivalente de clase. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Inicializa una nueva instancia de la clase [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | x | double | La coordenada x. |
|
|  | y | double | La coordenada y. |
|

### getX() {#getX--}
```
public double getX()
```


Obtiene la coordenada x.


**Returns:**
double - Un valor double que representa la coordenada x.

### getY() {#getY--}
```
public double getY()
```


Obtiene la coordenada y.


**Returns:**
double - Un valor double que representa la coordenada y.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Convierte la representación en cadena de un punto a su equivalente de clase. Un valor de retorno indica si la conversión se realizó con éxito o falló.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | s | java.lang.String | Una cadena que contiene un punto a convertir. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
