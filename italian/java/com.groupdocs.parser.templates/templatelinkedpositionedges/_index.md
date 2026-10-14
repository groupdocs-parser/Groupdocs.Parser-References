---
title: "TemplateLinkedPositionEdges"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce i bordi del campo collegato dove viene cercato il campo di testo."
type: docs
weight: 16
url: /it/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Fornisce i bordi del campo collegato dove il campo di testo è ricercato. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) è usato nella classe [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Inizializza una nuova istanza della classe [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Ottiene il valore che indica se l'istanza è vuota. |
|
|  | [isLeft()](#isLeft--) | Ottiene il valore che indica se un campo è ricercato a sinistra rispetto al campo collegato. |
|
|  | [isTop()](#isTop--) | Ottiene il valore che indica se un campo è ricercato in alto rispetto al campo collegato. |
|
|  | [isRight()](#isRight--) | Ottiene il valore che indica se un campo è ricercato a destra rispetto al campo collegato. |
|
|  | [isBottom()](#isBottom--) | Ottiene il valore che indica se un campo è ricercato in basso rispetto al campo collegato. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Converte la rappresentazione stringa dei bordi nella sua equivalente classe. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Inizializza una nuova istanza della classe [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | sinistra | boolean | Il valore che indica se un campo è ricercato a sinistra rispetto al campo collegato. |
|
|  | alto | boolean | Il valore che indica se un campo è ricercato in alto rispetto al campo collegato. |
|
|  | destra | boolean | Il valore che indica se un campo è ricercato dalla destra del campo collegato. |
|
|  | in basso | boolean | Il valore che indica se un campo è ricercato dal basso del campo collegato. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Ottiene il valore che indica se l'istanza è vuota.


**Returns:**
boolean -  true  se l'istanza è vuota (tutti i campi sono  false ); altrimenti,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Ottiene il valore che indica se un campo è ricercato a sinistra rispetto al campo collegato.


**Returns:**
boolean -  true  se un campo è ricercato da sinistra del campo collegato; altrimenti,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Ottiene il valore che indica se un campo è ricercato in alto rispetto al campo collegato.


**Returns:**
boolean -  true  se un campo è ricercato dall'alto del campo collegato; altrimenti,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Ottiene il valore che indica se un campo è ricercato a destra rispetto al campo collegato.


**Returns:**
boolean -  true  se un campo è ricercato da destra del campo collegato; altrimenti,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Ottiene il valore che indica se un campo è ricercato in basso rispetto al campo collegato.


**Returns:**
boolean -  true  se un campo è ricercato dal basso del campo collegato; altrimenti,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Converte la rappresentazione stringa dei bordi nella sua equivalente classe.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | s | java.lang.String | Una stringa che contiene i bordi da convertire. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
