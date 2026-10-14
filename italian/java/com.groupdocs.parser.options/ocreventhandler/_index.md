---
title: "OcrEventHandler"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce un gestore per gli eventi OCR."
type: docs
weight: 26
url: /it/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Fornisce un gestore per gli eventi OCR.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Inizializza una nuova istanza della classe [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Ottiene un elenco di messaggi di avviso. |
|
|  | [hasWarnings()](#hasWarnings--) | Ottiene il valore che indica se l'elenco degli avvisi non è vuoto. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Restituisce un elenco di messaggi di avviso per la pagina con pageIndex. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Imposta i messaggi di avviso per la pagina. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Inizializza una nuova istanza della classe [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Ottiene un elenco di messaggi di avviso.


**Returns:**
java.util.List<java.lang.String> - Un elenco di messaggi di avviso per tutte le pagine.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Ottiene il valore che indica se l'elenco degli avvisi non è vuoto.


**Returns:**
boolean -  true  se l'elenco degli avvisi non è vuoto; altrimenti,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Restituisce un elenco di messaggi di avviso per la pagina con pageIndex.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.util.List<java.lang.String> - Un elenco di messaggi di avviso per la pagina; elenco vuoto se non ci sono messaggi di avviso per la pagina.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Imposta i messaggi di avviso per la pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | L'elenco dei messaggi di avviso per la pagina. |
|

