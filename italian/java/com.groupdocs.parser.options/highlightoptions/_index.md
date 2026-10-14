---
title: "HighlightOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni che vengono utilizzate per estrarre un blocco di testo evidenziato intorno al testo trovato in scenari di ricerca."
type: docs
weight: 22
url: /it/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Fornisce le opzioni utilizzate per estrarre un'evidenziazione (un blocco di testo intorno al testo trovato in scenari di ricerca).

Un'istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) è usata come parametro nel metodo [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
Vedi gli esempi di utilizzo lì.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) senza limiti impostati. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) che viene usata per estrarre un'evidenziazione a lunghezza fissa. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) che viene usata per estrarre un'evidenziazione limitata alla riga. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) che viene usata per estrarre un'evidenziazione con un conteggio di parole fisso. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Ottiene una lunghezza massima del testo. |
|
|  | [getWordCount()](#getWordCount--) | Ottiene un conteggio massimo di parole. |
|
|  | [isLineLimited()](#isLineLimited--) | Ottiene il valore che indica se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Imposta una lunghezza massima del testo. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Imposta un conteggio massimo di parole. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Imposta il valore che indica se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) senza limiti impostati. Imposta almeno uno tra #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) prima di passare al parser.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) che viene usata per estrarre un'evidenziazione a lunghezza fissa.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | maxLength | int | La lunghezza massima del testo. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) che viene usata per estrarre un'evidenziazione limitata alla riga.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La lunghezza massima del testo. |
|
|  | isLineLimited | boolean | Il valore che indica se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) che viene usata per estrarre un'evidenziazione con un conteggio di parole fisso.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La lunghezza massima del testo. |
|
|  | wordCount | int | Il numero massimo di parole. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Inizializza una nuova istanza della classe [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La lunghezza massima del testo. |
|
|  | wordCount | java.lang.Integer | Il numero massimo di parole. |
|
|  | isLineLimited | boolean | Il valore che indica se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Ottiene una lunghezza massima del testo.


**Returns:**
java.lang.Integer - Un valore intero positivo che rappresenta la lunghezza massima del testo;  null  se la lunghezza del testo non è limitata.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Ottiene un conteggio massimo di parole.


**Returns:**
java.lang.Integer - Un valore intero positivo che rappresenta il conteggio massimo delle parole;  null  se il conteggio delle parole non è limitato.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Ottiene il valore che indica se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo.


**Returns:**
boolean -  true  se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo; altrimenti,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Imposta una lunghezza massima del testo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Un intero non negativo;  null  per rimuovere il limite di lunghezza. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Imposta un conteggio massimo di parole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Un intero non negativo;  null  per rimuovere il limite del conteggio delle parole. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Imposta il valore che indica se l'estrazione dell'evidenziazione è limitata dall'inizio (o dalla fine) di una riga di testo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lineLimited | boolean | true  per limitare ai limiti della riga. |
|

