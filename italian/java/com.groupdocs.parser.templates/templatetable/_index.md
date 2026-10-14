---
title: "TemplateTable"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce la tabella modello."
type: docs
weight: 20
url: /it/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Fornisce la tabella modello.

Esistono due modi per definire una tabella:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con il nome in MAIUSCOLO. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con il nome in MAIUSCOLO. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con il nome in MAIUSCOLO. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getLayout()](#getLayout--) | Restituisce il layout della tabella. |
|
|  | [getParameters()](#getParameters--) | Restituisce i parametri per rilevare la tabella in modalità automatica. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con il nome in MAIUSCOLO.

La tabella modello è impostata tramite layout della tabella se la tabella non può essere rilevata automaticamente:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Il layout della tabella. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con il nome in MAIUSCOLO.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Il layout della tabella. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Il layout della tabella. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Il layout della tabella. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) con il nome in MAIUSCOLO.

Se una tabella modello è impostata tramite parametri del rilevatore, la tabella viene rilevata automaticamente:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | I parametri per rilevare la tabella in modalità automatica. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | I parametri per rilevare la tabella in modalità automatica. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | I parametri per rilevare la tabella in modalità automatica. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | I parametri per rilevare la tabella in modalità automatica. |
|
|  | name | java.lang.String | Il nome della tabella. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui si trova la tabella modello;  null  se la tabella modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Restituisce il layout della tabella.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Restituisce i parametri per rilevare la tabella in modalità automatica.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
