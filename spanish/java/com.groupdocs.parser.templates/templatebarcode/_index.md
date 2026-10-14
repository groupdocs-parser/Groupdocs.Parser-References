---
title: "TemplateBarcode"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona el campo de código de barras de la plantilla."
type: docs
weight: 11
url: /es/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Proporciona el campo de código de barras de la plantilla.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que contiene el campo de código de barras de la plantilla. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el campo de código de barras de la plantilla. |
|
|  | nombre | java.lang.String | El nombre del campo de código de barras. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con el nombre en MAYÚSCULAS.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el campo de código de barras de la plantilla. |
|
|  | nombre | java.lang.String | El nombre del campo de código de barras. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con el nombre en MAYÚSCULAS.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el campo de código de barras de la plantilla. |
|
|  | nombre | java.lang.String | El nombre del campo de código de barras. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el campo de código de barras de la plantilla. |
|
|  | nombre | java.lang.String | El nombre del campo de código de barras. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el campo de código de barras de la plantilla. |
|
|  | nombre | java.lang.String | El nombre del campo de código de barras. |
|
|  | pageIndex | java.lang.Integer | Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que contiene el campo de código de barras de la plantilla.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

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
