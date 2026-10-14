---
title: "TemplateField"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce il campo di testo del modello."
type: docs
weight: 12
url: /it/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Fornisce il campo di testo del modello.

I campi di testo sono definiti dalla loro posizione sulla pagina. Ci sono tre modi per definire un campo di testo:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield) con il nome in MAIUSCOLO. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield) con il nome in MAIUSCOLO. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getPosition()](#getPosition--) | Ottiene il valore che descrive come trovare il campo del modello nella pagina del documento. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posizione del campo. |
|
|  | name | java.lang.String | Il nome del campo. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield) con il nome in MAIUSCOLO.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posizione del campo. |
|
|  | name | java.lang.String | Il nome del campo. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield) con il nome in MAIUSCOLO.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posizione del campo. |
|
|  | name | java.lang.String | Il nome del campo. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posizione del campo. |
|
|  | name | java.lang.String | Il nome del campo. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateField](../../com.groupdocs.parser/templates/templatefield).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La posizione del campo. |
|
|  | name | java.lang.String | Il nome del campo. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Ottiene il valore che descrive come trovare il campo del modello nella pagina del documento.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Crea una copia dell'elemento corrente con tutte le coordinate scalate del fattore specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fattore | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
