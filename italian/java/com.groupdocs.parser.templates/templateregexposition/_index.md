---
title: "TemplateRegexPosition"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce una posizione del campo del modello che utilizza l'espressione regolare."
type: docs
weight: 19
url: /it/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Fornisce una posizione del campo del modello che utilizza l'espressione regolare.

Il seguente esempio mostra la situazione se il documento contiene "Invoice Number INV-12345"
il campo del modello può essere definito nel modo seguente:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

In questo caso, come valore, viene estratta l'intera stringa. Per estrarre solo una parte della stringa
viene utilizzato il gruppo di espressione regolare "value":

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

In questo caso, come valore, viene estratta la stringa "INV-3337".

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Inizializza una nuova istanza della classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Inizializza una nuova istanza della classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getExpression()](#getExpression--) | Restituisce l'espressione regolare. |
|
|  | [isMatchCase()](#isMatchCase--) | Restituisce il valore che indica se il caso del testo non è ignorato. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Inizializza una nuova istanza della classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Inizializza una nuova istanza della classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Restituisce l'espressione regolare.


**Returns:**
java.lang.String - Una stringa che rappresenta l'espressione regolare.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Restituisce il valore che indica se il caso del testo non è ignorato.


**Returns:**
boolean -  true  se un caso di testo non è ignorato; altrimenti,  false .

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crea una copia della posizione corrente con tutte le coordinate scalate del fattore fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fattore | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
