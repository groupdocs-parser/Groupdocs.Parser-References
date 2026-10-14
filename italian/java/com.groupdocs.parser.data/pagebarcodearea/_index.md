---
title: "PageBarcodeArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'area barcode della pagina che è usata per rappresentare un valore barcode nella funzionalità di parsing tramite modello."
type: docs
weight: 18
url: /it/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Rappresenta un'area barcode della pagina che è usata per rappresentare un valore barcode nella funzionalità di parsing tramite modello.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getValue()](#getValue--) | Restituisce il valore del codice a barre. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Restituisce il nome del tipo di codice a barre. |
|
|  | [getConfidence()](#getConfidence--) | Restituisce il livello di confidenza del codice a barre analizzato. |
|
|  | [getAngle()](#getAngle--) | Restituisce l'angolo del codice a barre. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il valore del codice a barre. |
|
|  | codeTypeName | java.lang.String | Il nome del tipo del codice a barre. |
|
|  | confidenza | int | Il livello di confidenza del codice a barre analizzato. |
|
|  | angolo | double | L'angolo del codice a barre. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene l'area del codice a barre. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene l'area del codice a barre. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Restituisce il valore del codice a barre.


**Returns:**
java.lang.String - Un valore stringa che rappresenta un valore dell'area della pagina del codice a barre.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Restituisce il nome del tipo di codice a barre.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome del tipo del codice a barre.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Restituisce il livello di confidenza del codice a barre analizzato.


**Returns:**
int - Un valore intero che rappresenta la confidenza del codice a barre analizzato (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Restituisce l'angolo del codice a barre.


**Returns:**
double - Un valore intero che rappresenta l'angolo del codice a barre (0-360).

