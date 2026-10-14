---
title: "PageTextAreaOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione delle aree di testo della pagina."
type: docs
weight: 32
url: /it/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Fornisce le opzioni utilizzate per l'estrazione delle aree di testo della pagina.

Un'istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) è usata come parametro in [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
e i metodi [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) . Vedi gli esempi di utilizzo lì.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con valori predefiniti. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con l'opzione di utilizzo OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con la possibilità di impostare le opzioni OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con l'espressione regolare. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con l'espressione regolare e l'area rettangolare. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con l'espressione regolare, l'area rettangolare e la dimensione del bordo ignorato. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la dimensione del bordo ignorato. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getExpression()](#getExpression--) | Restituisce l'espressione regolare. |
|
|  | [isMatchCase()](#isMatchCase--) | Restituisce il valore che indica se il caso del testo non è ignorato. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Restituisce il valore che indica se i segmenti sono uniti. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Restituisce il valore che indica se la formattazione del testo è ignorata. |
|
|  | [isUseOcr()](#isUseOcr--) | Restituisce il valore che indica se il connettore OCR è usato per estrarre un testo. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Restituisce le opzioni aggiuntive per la funzionalità OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con valori predefiniti.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con l'opzione di utilizzo OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | useOcr | boolean | Il valore che indica se la funzionalità OCR è utilizzata per estrarre un testo. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con la possibilità di impostare le opzioni OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | useOcr | boolean | Il valore che indica se la funzionalità OCR è utilizzata per estrarre un testo. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Le opzioni aggiuntive per la funzionalità OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con l'espressione regolare. Le altre opzioni sono impostate per impostazione predefinita (vedi le note per i dettagli).

Le seguenti proprietà hanno valori predefiniti:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con l'espressione regolare e l'area rettangolare. Le altre opzioni sono impostate per impostazione predefinita (vedi le note per i dettagli).

Le seguenti proprietà hanno valori predefiniti:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene le aree della pagina. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con l'espressione regolare, l'area rettangolare e la dimensione del bordo ignorato. Le altre opzioni sono impostate per impostazione predefinita (vedi le note per i dettagli).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene le aree della pagina. |
|
|  | rectangleTolerance | double | La dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | uniteSegments | boolean | Il valore che indica se i segmenti sono uniti. |
|
|  | ignoreFormatting | boolean | Il valore che indica se la formattazione del testo è ignorata. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene le aree della pagina. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Inizializza una nuova istanza della classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la dimensione del bordo ignorato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | expression | java.lang.String | L'espressione regolare. |
|
|  | matchCase | boolean | Il valore che indica se il caso del testo non è ignorato. |
|
|  | uniteSegments | boolean | Il valore che indica se i segmenti sono uniti. |
|
|  | ignoreFormatting | boolean | Il valore che indica se la formattazione del testo è ignorata. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene le aree della pagina. |
|
|  | rectangleTolerance | double | La dimensione del bordo che viene ignorata quando catturata dall'area rettangolare. È misurata come frazione dell'altezza di un elemento di testo. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Restituisce l'espressione regolare.


**Returns:**
java.lang.String - Una stringa che rappresenta l'espressione regolare.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Restituisce il valore che indica se il caso del testo non è ignorato.


**Returns:**
boolean -  true  se un caso di testo non è ignorato; altrimenti,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Restituisce il valore che indica se i segmenti sono uniti.


**Returns:**
boolean - {code true} se i segmenti sono uniti; altrimenti, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Restituisce il valore che indica se la formattazione del testo è ignorata.


**Returns:**
boolean -  true  se la formattazione del testo è ignorata; altrimenti,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Restituisce il valore che indica se il connettore OCR è usato per estrarre un testo.


**Returns:**
boolean -  true  se la funzionalità OCR è utilizzata; altrimenti,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Restituisce le opzioni aggiuntive per la funzionalità OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

