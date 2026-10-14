---
title: "TemplateTable"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona la tabla de plantilla."
type: docs
weight: 20
url: /es/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Proporciona la tabla de plantilla.

Hay dos formas de definir una tabla:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con el nombre en MAYÚSCULAS. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getLayout()](#getLayout--) | Obtiene la disposición de la tabla. |
|
|  | [getParameters()](#getParameters--) | Obtiene los parámetros para detectar la tabla en modo automático. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con el nombre en MAYÚSCULAS.

La tabla de plantilla se establece mediante la disposición de la tabla si la tabla no puede detectarse automáticamente:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposición de la tabla. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con el nombre en MAYÚSCULAS.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposición de la tabla. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposición de la tabla. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposición de la tabla. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con el nombre en MAYÚSCULAS.

Si una tabla de plantilla se establece mediante parámetros del detector, la tabla se detecta automáticamente:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Los parámetros para detectar la tabla en modo automático. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Los parámetros para detectar la tabla en modo automático. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Los parámetros para detectar la tabla en modo automático. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inicializa una nueva instancia de la clase [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Los parámetros para detectar la tabla en modo automático. |
|
|  | nombre | java.lang.String | El nombre de la tabla. |
|
|  | pageIndex | java.lang.Integer | El índice de la página donde se encuentra la tabla de plantilla;  null  si la tabla de plantilla se encuentra en cualquier página. |
|
|  | pageWidth | java.lang.Double | El ancho de la página que se utilizó para crear el elemento de plantilla. |
|
|  | useUpperCaseName | boolean | El valor que indica si un  name  se convierte a MAYÚSCULAS. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Obtiene la disposición de la tabla.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Obtiene los parámetros para detectar la tabla en modo automático.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
