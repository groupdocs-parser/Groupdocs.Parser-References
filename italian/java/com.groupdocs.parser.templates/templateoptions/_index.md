---
title: "TemplateOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'analisi tramite la funzionalità del modello."
type: docs
weight: 17
url: /it/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Fornisce le opzioni utilizzate per l'analisi tramite la funzionalità del modello.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Inizializza una nuova istanza della classe [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Restituisce la dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Inizializza una nuova istanza della classe [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangleTolerance | double | La dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Restituisce la dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo.


**Returns:**
double - Il valore double da 0 (nessun bordo) a 1 (ignora l'intero elemento).

