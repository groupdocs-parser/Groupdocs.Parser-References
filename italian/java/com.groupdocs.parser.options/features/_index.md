---
title: "Funzionalità"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta l'elenco delle funzionalità supportate."
type: docs
weight: 18
url: /it/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Rappresenta l'elenco delle funzionalità supportate. Consente di ottenere informazioni su quali funzionalità sono supportate o meno per il documento.

Un'istanza di questa classe è utilizzata come proprietà [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). Vedi gli esempi d'uso lì.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Features()](#Features--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Restituisce il valore che indica se la funzionalità è supportata. |
|
|  | [isText()](#isText--) | Ottiene il valore che indica se l'estrazione del testo è supportata. |
|
|  | [isTextPage()](#isTextPage--) | Ottiene il valore che indica se l'estrazione della pagina di testo è supportata. |
|
|  | [isFormattedText()](#isFormattedText--) | Ottiene il valore che indica se l'estrazione del testo formattato è supportata. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Ottiene il valore che indica se l'estrazione della pagina di testo formattato è supportata. |
|
|  | [isSearch()](#isSearch--) | Ottiene il valore che indica se la ricerca di testo è supportata. |
|
|  | [isHighlight()](#isHighlight--) | Ottiene il valore che indica se l'estrazione dell'evidenziazione è supportata. |
|
|  | [isBarcodes()](#isBarcodes--) | Ottiene il valore che indica se l'estrazione dei codici a barre è supportata. |
|
|  | [isToc()](#isToc--) | Ottiene il valore che indica se l'estrazione del sommario è supportata. |
|
|  | [isMetadata()](#isMetadata--) | Ottiene il valore che indica se l'estrazione dei metadati è supportata. |
|
|  | [isContainer()](#isContainer--) | Ottiene il valore che indica se l'estrazione del contenitore è supportata. |
|
|  | [isTextAreas()](#isTextAreas--) | Ottiene il valore che indica se l'estrazione delle aree di testo è supportata. |
|
|  | [isStructure()](#isStructure--) | Ottiene il valore che indica se l'estrazione della struttura del testo è supportata. |
|
|  | [isImages()](#isImages--) | Ottiene il valore che indica se l'estrazione delle immagini è supportata. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Ottiene il valore che indica se l'estrazione dei collegamenti ipertestuali è supportata. |
|
|  | [isTables()](#isTables--) | Ottiene il valore che indica se l'estrazione delle tabelle è supportata. |
|
|  | [isAnnotations()](#isAnnotations--) | Ottiene il valore che indica se l'estrazione delle annotazioni è supportata. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Ottiene il valore che indica se l'analisi tramite modello è supportata. |
|
|  | [isParseForm()](#isParseForm--) | Ottiene il valore che indica se l'analisi dei moduli è supportata. |
|
|  | [isPreview()](#isPreview--) | Ottiene il valore che indica se la generazione dell'anteprima è supportata. |
|
|  | [isPagePreview()](#isPagePreview--) | Ottiene il valore che indica se la generazione dell'anteprima della pagina è supportata. |
|
|  | [isOcr()](#isOcr--) | Ottiene il valore che indica se la funzionalità OCR è supportata. |
|
|  | [isWorksheet()](#isWorksheet--) | Ottiene il valore che indica se l'estrazione del foglio di lavoro è supportata. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Restituisce il valore che indica se la funzionalità è supportata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | featureName | java.lang.String | Il nome della funzionalità. |
|

**Returns:**
boolean -  true  se la funzionalità è supportata; altrimenti,  false .

### isText() {#isText--}
```
public boolean isText()
```


Ottiene il valore che indica se l'estrazione del testo è supportata.


**Returns:**
boolean -  true  se l'estrazione del testo è supportata; altrimenti,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Ottiene il valore che indica se l'estrazione della pagina di testo è supportata.


**Returns:**
boolean -  true  se l'estrazione della pagina di testo è supportata; altrimenti,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Ottiene il valore che indica se l'estrazione del testo formattato è supportata.


**Returns:**
boolean -  true  se l'estrazione del testo formattato è supportata; altrimenti,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Ottiene il valore che indica se l'estrazione della pagina di testo formattato è supportata.


**Returns:**
boolean -  true  se la pagina di testo formattato è supportata; altrimenti,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Ottiene il valore che indica se la ricerca di testo è supportata.


**Returns:**
boolean -  true  se la ricerca del testo è supportata; altrimenti,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Ottiene il valore che indica se l'estrazione dell'evidenziazione è supportata.


**Returns:**
boolean -  true  se l'estrazione dell'evidenziazione è supportata; altrimenti,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Ottiene il valore che indica se l'estrazione dei codici a barre è supportata.


**Returns:**
boolean -  true  se l'estrazione dei codici a barre è supportata; altrimenti,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Ottiene il valore che indica se l'estrazione del sommario è supportata.


**Returns:**
boolean -  true  se l'estrazione del sommario è supportata; altrimenti,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Ottiene il valore che indica se l'estrazione dei metadati è supportata.


**Returns:**
boolean -  true  se l'estrazione dei metadati è supportata; altrimenti,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Ottiene il valore che indica se l'estrazione del contenitore è supportata.


**Returns:**
boolean -  true  se l'estrazione del contenitore è supportata; altrimenti,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Ottiene il valore che indica se l'estrazione delle aree di testo è supportata.


**Returns:**
boolean -  true  se l'estrazione delle aree di testo è supportata; altrimenti,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Ottiene il valore che indica se l'estrazione della struttura del testo è supportata.


**Returns:**
boolean -  true  se l'estrazione della struttura del testo è supportata; altrimenti,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Ottiene il valore che indica se l'estrazione delle immagini è supportata.


**Returns:**
boolean -  true  se l'estrazione delle immagini è supportata; altrimenti,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Ottiene il valore che indica se l'estrazione dei collegamenti ipertestuali è supportata.


**Returns:**
boolean -  true  se l'estrazione dei collegamenti ipertestuali è supportata; altrimenti,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Ottiene il valore che indica se l'estrazione delle tabelle è supportata.


**Returns:**
boolean -  true  se l'estrazione delle tabelle è supportata; altrimenti,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Ottiene il valore che indica se l'estrazione delle annotazioni è supportata.


**Returns:**
boolean -  true  se l'estrazione delle annotazioni è supportata; altrimenti,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Ottiene il valore che indica se l'analisi tramite modello è supportata.


**Returns:**
boolean -  true  se l'analisi tramite modello è supportata; altrimenti,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Ottiene il valore che indica se l'analisi dei moduli è supportata.


**Returns:**
boolean -  true  se l'analisi del modulo è supportata; altrimenti,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Ottiene il valore che indica se la generazione dell'anteprima è supportata.


**Returns:**
boolean -  true  se la generazione dell'anteprima è supportata; altrimenti,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Ottiene il valore che indica se la generazione dell'anteprima della pagina è supportata.


**Returns:**
boolean -  true  se la generazione dell'anteprima della pagina è supportata; altrimenti,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Ottiene il valore che indica se la funzionalità OCR è supportata.


**Returns:**
boolean -  true  se la funzionalità OCR è supportata; altrimenti,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Ottiene il valore che indica se l'estrazione del foglio di lavoro è supportata.


**Returns:**
boolean -  true  se l'estrazione del foglio di lavoro è supportata; altrimenti,  false .

