---
title: "TemplateRegexPosition"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona una posición de campo de plantilla que utiliza la expresión regular."
type: docs
weight: 19
url: /es/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Proporciona una posición de campo de plantilla que utiliza la expresión regular.

El siguiente ejemplo muestra la situación si el documento contiene "Invoice Number INV-12345"
entonces el campo de plantilla puede definirse de la siguiente manera:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

En este caso, como valor se extrae la cadena completa. Para extraer solo una parte de la cadena
se utiliza el grupo de expresión regular "value":

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

En este caso, como valor se extrae la cadena "INV-3337".

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Inicializa una nueva instancia de la clase [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Inicializa una nueva instancia de la clase [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getExpression()](#getExpression--) | Obtiene la expresión regular. |
|
|  | [isMatchCase()](#isMatchCase--) | Obtiene el valor que indica si no se ignora la distinción de mayúsculas y minúsculas del texto. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Inicializa una nueva instancia de la clase [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Inicializa una nueva instancia de la clase [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Obtiene la expresión regular.


**Returns:**
java.lang.String - Una cadena que representa la expresión regular.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Obtiene el valor que indica si no se ignora la distinción de mayúsculas y minúsculas del texto.


**Returns:**
boolean -  true  si una distinción de mayúsculas y minúsculas no se ignora; de lo contrario,  false .

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
