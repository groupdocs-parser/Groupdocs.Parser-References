---
title: "TextOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione di testo."
type: docs
weight: 37
url: /it/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Fornisce le opzioni utilizzate per l'estrazione di testo.

Un'istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) è usata come parametro in [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
e i metodi [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-). Vedi gli esempi d'uso lì.

Viene usato per specificare la modalità raw di estrazione del testo. Un testo in questa modalità viene estratto in modo non accurato
ma più veloce rispetto alla modalità standard. Se la modalità raw non supporta il formato del documento,
questo parametro viene ignorato e viene usata la modalità standard.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con l'opzione di utilizzo OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con la possibilità di impostare le opzioni OCR. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Restituisce il valore che indica se la modalità raw è utilizzata. |
|
|  | [isUseOcr()](#isUseOcr--) | Restituisce il valore che indica se il connettore OCR è usato per estrarre un testo. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Restituisce le opzioni aggiuntive per la funzionalità OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Restituisce il valore che indica se le annotazioni sono incluse nel testo estratto. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Imposta il valore che indica se le annotazioni sono incluse nel testo estratto. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Il valore che indica se la modalità raw è utilizzata. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con l'opzione di utilizzo OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Il valore che indica se la modalità raw è utilizzata. |
|
|  | useOcr | boolean | Il valore che indica se la funzionalità OCR è utilizzata per estrarre un testo. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Inizializza una nuova istanza della classe [TextOptions](../../com.groupdocs.parser.options/textoptions) con la possibilità di impostare le opzioni OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Il valore che indica se la modalità raw è utilizzata. |
|
|  | useOcr | boolean | Il valore che indica se la funzionalità OCR è utilizzata per estrarre un testo. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Le opzioni aggiuntive per la funzionalità OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Restituisce il valore che indica se la modalità raw è utilizzata.


**Returns:**
boolean -  true  se la modalità raw è utilizzata; altrimenti,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Restituisce il valore che indica se le annotazioni sono incluse nel testo estratto. Il valore predefinito è  false .


**Returns:**
boolean -  true  se le annotazioni sono incluse; altrimenti,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Imposta il valore che indica se le annotazioni sono incluse nel testo estratto.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  per includere le annotazioni nel testo estratto. |
|

