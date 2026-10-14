---
title: "TemplateLinkedPosition"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce una posizione del campo del modello che utilizza il campo collegato."
type: docs
weight: 15
url: /it/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Fornisce una posizione del campo del modello che utilizza il campo collegato.

Il seguente esempio mostra il codice per la situazione in cui è noto che il campo con il numero della fattura
è posizionato a destra della stringa "Invoice number", viene utilizzato il seguente codice:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Inizializza una nuova istanza della classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Inizializza una nuova istanza della classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) con nome in MAIUSCOLO. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Inizializza una nuova istanza della classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Restituisce il nome del campo collegato. |
|
|  | [getSearchArea()](#getSearchArea--) | Restituisce la dimensione dell'area in cui viene cercato un campo. |
|
|  | [isAutoScale()](#isAutoScale--) | Restituisce il valore che indica se  SearchArea  è scalata in base alle dimensioni del campo collegato. |
|
|  | [getEdges()](#getEdges--) | Restituisce i bordi del campo collegato in cui viene cercato un campo. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Inizializza una nuova istanza della classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Il nome del campo collegato. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | La dimensione dell'area in cui viene cercato un campo. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | I bordi del campo collegato in cui viene cercato un campo. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Inizializza una nuova istanza della classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) con nome in MAIUSCOLO.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Il nome del campo collegato. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | La dimensione dell'area in cui viene cercato un campo. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | I bordi del campo collegato in cui viene cercato un campo. |
|
|  | autoScale | boolean | Il valore che indica se searchArea è scalato dalla dimensione del campo collegato. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Il nome del campo collegato. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | La dimensione dell'area in cui viene cercato un campo. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | I bordi del campo collegato in cui viene cercato un campo. |
|
|  | autoScale | boolean | Il valore che indica se searchArea è scalato dalla dimensione del campo collegato.\\ |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Restituisce il nome del campo collegato.


**Returns:**
java.lang.String - Un valore stringa in maiuscolo che rappresenta il nome del campo collegato.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Restituisce la dimensione dell'area in cui viene cercato un campo.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Restituisce il valore che indica se  SearchArea  è scalata in base alle dimensioni del campo collegato.


**Returns:**
java.lang.Boolean - {code true} se  SearchArea  è scalato dalla dimensione del campo collegato; altrimenti,  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Restituisce i bordi del campo collegato in cui viene cercato un campo.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

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
