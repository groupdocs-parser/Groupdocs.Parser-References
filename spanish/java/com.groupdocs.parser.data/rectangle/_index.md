---
title: "Rectangle"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un área rectangular."
type: docs
weight: 26
url: /es/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Representa un área rectangular.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Inicializa una nueva instancia de la clase [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Inicializa una nueva instancia de la clase [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getLeft()](#getLeft--) | Obtiene la coordenada x del borde izquierdo del área rectangular. |
|
|  | [getTop()](#getTop--) | Obtiene la coordenada y del borde superior del área rectangular. |
|
|  | [getRight()](#getRight--) | Obtiene la coordenada x del borde derecho del área rectangular. |
|
|  | [getBottom()](#getBottom--) | Obtiene la coordenada y del borde inferior del área rectangular. |
|
|  | [getPosition()](#getPosition--) | Obtiene las coordenadas de la esquina superior izquierda del área rectangular. |
|
|  | [getSize()](#getSize--) | Obtiene el tamaño. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Inicializa una nueva instancia de la clase [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | izquierda | double | La coordenada x del borde izquierdo del área rectangular. |
|
|  | arriba | double | La coordenada y del borde superior del área rectangular. |
|
|  | derecha | double | La coordenada x del borde derecho del área rectangular. |
|
|  | inferior | double | La coordenada y del borde inferior del área rectangular. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Inicializa una nueva instancia de la clase [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Las coordenadas de la esquina superior izquierda del área rectangular. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | El tamaño del área rectangular. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Obtiene la coordenada x del borde izquierdo del área rectangular.


**Returns:**
double - Un valor double que representa la coordenada x del borde izquierdo del área rectangular.

### getTop() {#getTop--}
```
public double getTop()
```


Obtiene la coordenada y del borde superior del área rectangular.


**Returns:**
double - Un valor double que representa la coordenada y del borde superior del área rectangular.

### getRight() {#getRight--}
```
public double getRight()
```


Obtiene la coordenada x del borde derecho del área rectangular.


**Returns:**
double - Un valor double que representa la coordenada x del borde derecho del área rectangular.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Obtiene la coordenada y del borde inferior del área rectangular.


**Returns:**
double - Un valor double que representa la coordenada y del borde inferior del área rectangular.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Obtiene las coordenadas de la esquina superior izquierda del área rectangular.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Obtiene el tamaño.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
