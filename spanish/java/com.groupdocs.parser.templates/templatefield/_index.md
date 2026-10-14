---
title: "TemplateField"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona el campo de texto de la plantilla."
type: docs
weight: 12
url: /es/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Proporciona el campo de texto de la plantilla.

Los campos de texto se definen por su posición en la página. Hay tres formas de definir un campo de texto:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getPosition()](#getPosition--) | Obtiene el valor que describe cómo encontrar el campo de plantilla en la página del documento. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posición del campo. |
|
|  | nombre | java.lang.String | El nombre del campo. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield) con el nombre en MAYÚSCULAS.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posición del campo. |
|
|  | nombre | java.lang.String | El nombre del campo. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield) con el nombre en MAYÚSCULAS.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posición del campo. |
|
|  | nombre | java.lang.String | El nombre del campo. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posición del campo. |
|
|  | nombre | java.lang.String | El nombre del campo. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posición del campo. |
|
|  | nombre | java.lang.String | El nombre del campo. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Obtiene el valor que describe cómo encontrar el campo de plantilla en la página del documento.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Crea una copia del elemento actual con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
