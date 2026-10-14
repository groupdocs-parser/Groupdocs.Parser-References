---
title: "TemplateFixedPosition"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona una posición de campo de plantilla que se define por el área rectangular."
type: docs
weight: 13
url: /es/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Proporciona una posición de campo de plantilla que se define por el área rectangular.

Esta es la forma más sencilla de definir la posición del campo. Requiere establecer un área rectangular en la página que delimita
el valor del campo. Todo el texto que esté contenido (incluso parcialmente) en el área rectangular será extraído como un valor:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que contiene el campo de plantilla. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el campo de plantilla. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que contiene el campo de plantilla.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crea una copia de la posición actual con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
