---
title: "BarcodeOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione dei codici a barre."
type: docs
weight: 10
url: /it/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Fornisce le opzioni utilizzate per l'estrazione dei codici a barre.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Inizializza una nuova istanza della classe BarcodeOptions con valori predefiniti. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe BarcodeOptions con l'area rettangolare. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Inizializza una nuova istanza della classe BarcodeOptions con impostazioni di qualità e tipi di codice. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Inizializza una nuova istanza della classe BarcodeOptions. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Restituisce il valore che indica se i codici a barre errati sono consentiti. |
|
|  | [getDimension()](#getDimension--) | Restituisce la dimensione minima dell'elemento minimo del codice a barre. |
|
|  | [getImageQuality()](#getImageQuality--) | Restituisce la qualità di un'immagine sorgente. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Restituisce la qualità di un codice a barre sorgente. |
|
|  | [getRectangle()](#getRectangle--) | Restituisce l'area rettangolare che contiene le aree della pagina. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Restituisce i tipi di codici a barre da leggere. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Imposta il valore che indica se i codici a barre errati sono consentiti. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Imposta la dimensione minima dell'elemento minimo del codice a barre. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Imposta la qualità di un'immagine sorgente. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Imposta la qualità di un codice a barre sorgente. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Imposta l'area rettangolare che contiene i codici a barre. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Imposta i tipi di codici a barre da leggere. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Inizializza una nuova istanza della classe BarcodeOptions con valori predefiniti.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Inizializza una nuova istanza della classe BarcodeOptions con l'area rettangolare.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene i codici a barre. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Inizializza una nuova istanza della classe BarcodeOptions con impostazioni di qualità e tipi di codice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualità di un'immagine di origine. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualità di un codice a barre di origine. |
|
|  | codeTypes | java.lang.String[] | I tipi di codici a barre da leggere. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Inizializza una nuova istanza della classe BarcodeOptions.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene i codici a barre. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualità di un'immagine di origine. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualità di un codice a barre di origine. |
|
|  | dimension | java.lang.Float | La dimensione minima dell'elemento minimo del codice a barre. |
|
|  | allowIncorrectBarcodes | boolean | Il valore che indica se i codici a barre errati sono consentiti. |
|
|  | codeTypes | java.lang.String[] | I tipi di codici a barre da leggere. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Restituisce il valore che indica se i codici a barre errati sono consentiti.


**Returns:**
boolean -  true  se i codici a barre errati sono consentiti; altrimenti,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Restituisce la dimensione minima dell'elemento minimo del codice a barre.


**Returns:**
java.lang.Float - Il valore float che rappresenta l'elemento minimo del codice a barre;  null  se è usata la modalità automatica.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Restituisce la qualità di un'immagine sorgente.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Restituisce la qualità di un codice a barre sorgente.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Restituisce l'area rettangolare che contiene le aree della pagina.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Restituisce i tipi di codici a barre da leggere.


**Returns:**
java.util.List<java.lang.String> - La collezione di sola lettura che contiene i tipi di codici a barre da leggere; collezione vuota se non è impostata.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Imposta il valore che indica se i codici a barre errati sono consentiti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  se i codici a barre errati sono consentiti. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Imposta la dimensione minima dell'elemento minimo del codice a barre.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dimension | java.lang.Float | L'elemento minimo del codice a barre;  null  per la modalità automatica. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Imposta la qualità di un'immagine sorgente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La modalità di qualità dell'immagine. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Imposta la qualità di un codice a barre sorgente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La modalità di qualità del codice a barre. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Imposta l'area rettangolare che contiene i codici a barre.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare;  null  per scansionare l'intera pagina. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Imposta i tipi di codici a barre da leggere.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | I tipi di codici a barre;  null  o vuoto per tutti i tipi. |
|

