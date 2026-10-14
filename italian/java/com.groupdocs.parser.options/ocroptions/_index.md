---
title: "OcrOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per il connettore OCR."
type: docs
weight: 27
url: /it/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Fornisce le opzioni utilizzate per il connettore OCR.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con valori predefiniti. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con area rettangolare. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con opzioni di anteprima pagina. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con l'oggetto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con area rettangolare e l'oggetto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Restituisce l'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
|
|  | [getHandler()](#getHandler--) | Restituisce il gestore degli eventi per catturare gli eventi OCR. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Ottiene il valore che indica se il correttore ortografico è utilizzato. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Ottiene le opzioni di anteprima della pagina utilizzate per renderizzare la pagina fornita al motore OCR. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Imposta le opzioni di anteprima della pagina utilizzate per renderizzare la pagina fornita al motore OCR. |
|
|  | [getLanguage()](#getLanguage--) | Ottiene la lingua utilizzata per il riconoscimento ottico dei caratteri. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Imposta la lingua utilizzata per il riconoscimento ottico dei caratteri. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Imposta l'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Imposta il gestore di eventi per catturare gli eventi OCR. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Imposta il valore che indica se il correttore ortografico è utilizzato. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con valori predefiniti.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con area rettangolare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con opzioni di anteprima pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Le opzioni utilizzate per renderizzare l'anteprima della pagina fornita al motore OCR. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con l'oggetto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Un'istanza di [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) per catturare gli eventi OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con area rettangolare e l'oggetto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Un'istanza di [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) per catturare gli eventi OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Inizializza una nuova istanza della classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Un'istanza di [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) per catturare gli eventi OCR. |
|
|  | useSpellCheker | boolean | Il valore che indica se il correttore ortografico è utilizzato. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Restituisce l'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Restituisce il gestore degli eventi per catturare gli eventi OCR.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Ottiene il valore che indica se il correttore ortografico è utilizzato.


**Returns:**
boolean -  true  se il correttore ortografico è utilizzato; altrimenti,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Ottiene le opzioni di anteprima della pagina utilizzate per renderizzare la pagina fornita al motore OCR.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Imposta le opzioni di anteprima della pagina utilizzate per renderizzare la pagina fornita al motore OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Le opzioni di anteprima della pagina. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Ottiene la lingua utilizzata per il riconoscimento ottico dei caratteri.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Imposta la lingua utilizzata per il riconoscimento ottico dei caratteri.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | Il valore enum [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Imposta l'area rettangolare che limita l'area della pagina utilizzata per il riconoscimento del testo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Il rettangolo, o  null  per scansionare l'intera pagina. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Imposta il gestore di eventi per catturare gli eventi OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Il gestore di eventi. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Imposta il valore che indica se il correttore ortografico è utilizzato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  per abilitare il controllo ortografico. |
|

