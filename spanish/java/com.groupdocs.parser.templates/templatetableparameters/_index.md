---
title: "TemplateTableParameters"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona parámetros para los algoritmos de detección de tablas."
type: docs
weight: 22
url: /es/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Proporciona parámetros para los algoritmos de detección de tablas.

Hay dos algoritmos para detectar una tabla:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

En algunos casos, cuando los algoritmos no pueden detectar una tabla o lo hacen de manera no precisa, se utiliza la clase [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Inicializa una nueva instancia de la clase [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Inicializa una nueva instancia de la clase [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que contiene la tabla. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Obtiene los separadores de columnas de la tabla. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Obtiene el valor que indica si la tabla tiene celdas combinadas. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Obtiene el número mínimo de filas de la tabla. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Obtiene el número mínimo de columnas de la tabla. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Obtiene el espacio mínimo entre las columnas de la tabla. |
|
|  | [scale(double factor)](#scale-double-) | Crea una copia de estos parámetros con todas las coordenadas escaladas por el factor dado. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Inicializa una nueva instancia de la clase [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene la tabla. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Los separadores de columnas de la tabla. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Inicializa una nueva instancia de la clase [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene la tabla. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Los separadores de columnas de la tabla. |
|
|  | mergedCells | java.lang.Boolean | El valor que indica si la tabla tiene celdas combinadas. |
|
|  | minRowCount | java.lang.Integer | El número mínimo de filas de la tabla. |
|
|  | minColumnCount | java.lang.Integer | El número mínimo de columnas de la tabla. |
|
|  | minVerticalSpace | java.lang.Integer | El espacio mínimo entre las columnas de la tabla. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que contiene la tabla.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Obtiene los separadores de columnas de la tabla.


**Returns:**
java.util.List<java.lang.Double> - Una colección de valores double que representan las coordenadas x de los separadores de columnas de la tabla;  null  si no está configurado.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Obtiene el valor que indica si la tabla tiene celdas combinadas.


**Returns:**
java.lang.Boolean -  true  si la tabla tiene celdas combinadas; de lo contrario,  false .  null  si no está configurado.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Obtiene el número mínimo de filas de la tabla.


**Returns:**
java.lang.Integer - Un valor entero que representa el número mínimo de filas de la tabla;  null  si no está configurado.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Obtiene el número mínimo de columnas de la tabla.


**Returns:**
java.lang.Integer - Un valor entero que representa el número mínimo de columnas de la tabla;  null  si no está configurado.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Obtiene el espacio mínimo entre las columnas de la tabla.


**Returns:**
java.lang.Integer - Un valor entero que representa el espacio mínimo entre las columnas de la tabla;  null  si no está configurado.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Crea una copia de estos parámetros con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | factor | double | El factor de escala. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

