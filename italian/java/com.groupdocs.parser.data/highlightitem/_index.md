---
title: "HighlightItem"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'evidenziazione di una parte del testo solitamente utilizzata per spiegare il contesto del testo trovato nella funzionalità di ricerca."
type: docs
weight: 14
url: /it/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Rappresenta un evidenziatore, una parte del testo solitamente usata per spiegare il contesto del testo trovato nella funzionalità di ricerca.

Un'istanza della classe [HighlightItem](../../com.groupdocs.parser.data/highlightitem) è utilizzata come valore di ritorno del metodo [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-),
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Inizializza una nuova istanza della classe [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getPosition()](#getPosition--) | Restituisce la posizione nel testo del documento. |
|
|  | [getText()](#getText--) | Restituisce il testo dell'evidenziazione. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Inizializza una nuova istanza della classe [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | posizione | int | La posizione nel testo del documento. |
|
|  | testo | java.lang.String | Il testo dell'evidenziazione. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Restituisce la posizione nel testo del documento.


**Returns:**
int - Un indice basato su zero della posizione iniziale dell'evidenziazione.

### getText() {#getText--}
```
public String getText()
```


Restituisce il testo dell'evidenziazione.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il testo dell'evidenziazione.

