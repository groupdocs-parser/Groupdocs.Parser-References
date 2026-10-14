---
title: "TemplateTableLayout"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona el diseño de tabla de plantilla que es utilizado por la clase para definir la posición de la tabla."
type: docs
weight: 21
url: /es/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Proporciona el diseño de tabla de plantilla que es utilizado por la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) para definir la posición de la tabla.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Inicializa una nueva instancia de la clase [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que contiene la tabla. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Obtiene los separadores de columnas de la tabla. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Obtiene los separadores de filas de la tabla. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Crea un nuevo diseño con el mismo tamaño, separadores y posición en el punto. |
|
|  | [scale(double factor)](#scale-double-) | Crea una copia de este diseño con todas las coordenadas escaladas por el factor dado. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Inicializa una nueva instancia de la clase [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Los separadores de columnas de la tabla. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Los separadores de filas de la tabla. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que contiene la tabla.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Obtiene los separadores de columnas de la tabla.


**Returns:**
java.util.List<java.lang.Double> - Una colección de valores double que representan las coordenadas x de los separadores de columnas de la tabla.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Obtiene los separadores de filas de la tabla.


**Returns:**
java.util.List<java.lang.Double> - Una colección de valores double que representan las coordenadas y de los separadores de filas de la tabla.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Crea un nuevo diseño con el mismo tamaño, separadores y posición en el punto.

Esta funcionalidad permite mover el diseño de tabla.

Por ejemplo, un documento tiene tablas en cada página (o un conjunto de documentos con una tabla en la página).
Estas tablas difieren en posición y contenido, pero tienen las mismas columnas y filas. En este caso, un usuario
puede definir el objeto [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) en (0, 0) una vez y luego moverlo a la ubicación de la tabla definitiva.

Si la posición de la tabla depende de otro objeto de la página, un usuario puede definir el objeto [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)
basado en el documento plantilla y luego moverlo según un objeto ancla. Por ejemplo, si esta es una tabla de resumen
y le sigue una tabla de detalles (que puede contener un número diferente de filas). En este caso, un usuario puede definir
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
método devuelve una copia del objeto actual. Un usuario puede pasar cualquier coordenada
(incluso negativas - entonces el diseño se moverá a la izquierda/arriba).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | La posición del nuevo diseño. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Crea una copia de este diseño con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | factor | double | El factor de escala. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

