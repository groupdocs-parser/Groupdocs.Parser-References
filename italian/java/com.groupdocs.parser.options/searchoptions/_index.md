---
title: "SearchOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per la ricerca di testo."
type: docs
weight: 35
url: /it/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Fornisce le opzioni utilizzate per la ricerca di testo.

Un'istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) è usata come parametro nel metodo [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Vedi gli esempi di utilizzo lì.

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca con le opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca con le stesse opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca senza estrazione dell'evidenziazione. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca per pagine e senza estrazione dell'evidenziazione. |
|
|  | [SearchOptions()](#SearchOptions--) | Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) con valori predefiniti. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Restituisce il valore che indica se il caso del testo non è ignorato. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Restituisce il valore che indica se la ricerca di testo è limitata a parole intere. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Restituisce il valore che indica se viene utilizzata un'espressione regolare. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Restituisce il valore che indica se la ricerca è eseguita per pagine. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Restituisce le opzioni per l'evidenziazione sinistra. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Restituisce le opzioni per l'evidenziazione destra. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Restituisce il valore che rappresenta l'indice massimo della pagina da cercare. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | matchWholeWord | boolean | Il valore che indica se la ricerca del testo è limitata a una parola intera. |
|
|  | useRegularExpression | boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
|
|  | searchByPages | boolean | Il valore che indica se la ricerca viene eseguita per pagine. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per l'evidenziazione a sinistra. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per l'evidenziazione a destra. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | matchWholeWord | boolean | Il valore che indica se la ricerca del testo è limitata a una parola intera. |
|
|  | useRegularExpression | boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
|
|  | maxPageIndex | int | Il valore che rappresenta l'indice massimo della pagina da cercare |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per l'evidenziazione a sinistra. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per l'evidenziazione a destra. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca con le opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | matchWholeWord | boolean | Il valore che indica se la ricerca del testo è limitata a una parola intera. |
|
|  | useRegularExpression | boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per l'evidenziazione a sinistra. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per l'evidenziazione a destra. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca con le stesse opzioni di evidenziazione per l'estrazione dell'evidenziazione sinistra e destra.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | matchWholeWord | boolean | Il valore che indica se la ricerca del testo è limitata a una parola intera. |
|
|  | useRegularExpression | boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni per entrambe le evidenziazioni. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca senza estrazione dell'evidenziazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | matchWholeWord | boolean | Il valore che indica se la ricerca del testo è limitata a una parola intera. |
|
|  | useRegularExpression | boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) che è usata per la ricerca per pagine e senza estrazione dell'evidenziazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | matchWholeWord | boolean | Il valore che indica se la ricerca del testo è limitata a una parola intera. |
|
|  | useRegularExpression | boolean | Il valore che indica se viene utilizzata un'espressione regolare. |
|
|  | searchByPages | boolean | Il valore che indica se la ricerca viene eseguita per pagine. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Inizializza una nuova istanza della classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) con valori predefiniti. Vedi le note per i dettagli.

Le seguenti proprietà hanno valori predefiniti:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Restituisce il valore che indica se il caso del testo non è ignorato.


**Returns:**
boolean -  true  se un caso di testo non è ignorato; altrimenti,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Restituisce il valore che indica se la ricerca di testo è limitata a parole intere.


**Returns:**
boolean -  true  se la ricerca del testo è limitata a una parola intera; altrimenti,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Restituisce il valore che indica se viene utilizzata un'espressione regolare.


**Returns:**
boolean -  true  se viene utilizzata un'espressione regolare; altrimenti,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Restituisce il valore che indica se la ricerca è eseguita per pagine.


**Returns:**
boolean -  true  se la ricerca viene eseguita per pagine; altrimenti,  false  e la ricerca viene eseguita sull'intero documento senza includere il valore della proprietà [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) nella classe [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Restituisce le opzioni per l'evidenziazione sinistra.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Restituisce le opzioni per l'evidenziazione destra.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Restituisce il valore che rappresenta l'indice massimo della pagina da cercare.


**Returns:**
int - Un valore intero che rappresenta l'indice massimo della pagina da cercare; -1 se non impostato;

