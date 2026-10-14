---
title: "OcrConnectorBase"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce la funzionalità OCR."
type: docs
weight: 25
url: /it/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Fornisce la funzionalità OCR.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Inizializza una nuova istanza della classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Restituisce il valore che indica se l'estrazione del testo è supportata. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Restituisce il valore che indica se l'estrazione delle aree di testo è supportata. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Riconosce un testo dal flusso imageStream. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Riconosce le aree di testo dal flusso imageStream. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Inizializza una nuova istanza della classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Restituisce il valore che indica se l'estrazione del testo è supportata.


**Returns:**
boolean -  true  se l'estrazione del testo è supportata; altrimenti,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Restituisce il valore che indica se l'estrazione delle aree di testo è supportata.


**Returns:**
boolean -  true  se l'estrazione delle aree di testo è supportata; altrimenti,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Riconosce un testo dal flusso imageStream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | La rappresentazione immagine della pagina del documento. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Le opzioni OCR. |
|

**Returns:**
java.lang.String - Una stringa che rappresenta un testo riconosciuto;  null  se il riconoscimento del testo non è supportato.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Riconosce le aree di testo dal flusso imageStream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | La rappresentazione immagine della pagina del documento. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | La dimensione della pagina del documento. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Le opzioni OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Una collezione di oggetti [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  se il riconoscimento delle aree di testo non è supportato.

