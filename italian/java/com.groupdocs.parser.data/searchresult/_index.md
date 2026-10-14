---
title: "SearchResult"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta il risultato della ricerca nella funzionalità di ricerca."
type: docs
weight: 27
url: /it/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Rappresenta il risultato della ricerca nella funzionalità di ricerca.

Un'istanza della classe SearchResult è utilizzata come valore di ritorno di [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-)
e i metodi [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) . Vedi gli esempi d'uso lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Inizializza una nuova istanza della classe [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Inizializza una nuova istanza della classe [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getPosition()](#getPosition--) | Restituisce la posizione nel testo del documento. |
|
|  | [getText()](#getText--) | Restituisce il testo. |
|
|  | [getPageIndex()](#getPageIndex--) | Restituisce l'indice della pagina in cui è trovato il testo. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Restituisce l'evidenziazione sinistra. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Restituisce l'evidenziazione destra. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Inizializza una nuova istanza della classe [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | posizione | int | La posizione nel testo del documento. |
|
|  | testo | java.lang.String | Il testo trovato. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui è trovato il testo. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | L'evidenziazione sinistra. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | L'evidenziazione destra. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Inizializza una nuova istanza della classe [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | posizione | int | La posizione nel testo del documento. |
|
|  | testo | java.lang.String | Il testo trovato. |
|
|  | pageIndex | java.lang.Integer | L'indice della pagina in cui è trovato il testo. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Restituisce la posizione nel testo del documento.


**Returns:**
int - Un indice basato su zero della posizione iniziale del risultato della ricerca.

### getText() {#getText--}
```
public String getText()
```


Restituisce il testo.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il testo trovato.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Restituisce l'indice della pagina in cui è trovato il testo.


**Returns:**
java.lang.Integer - Un indice basato su zero della pagina in cui è trovato il testo; null se la ricerca è eseguita sull'intero testo del documento.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Restituisce l'evidenziazione sinistra.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Restituisce l'evidenziazione destra.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

