---
title: "PreviewOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima."
type: docs
weight: 34
url: /it/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Fornisce opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Inizializza una nuova istanza della classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) causando la chiusura del flusso di output. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Inizializza una nuova istanza della classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) facendo restituire il flusso di output al client per un uso successivo. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getWidth()](#getWidth--) | Restituisce la larghezza dell'anteprima della pagina. |
|
|  | [setWidth(int width)](#setWidth-int-) | Imposta la larghezza dell'anteprima della pagina. |
|
|  | [getHeight()](#getHeight--) | Ottiene l'altezza dell'anteprima della pagina. |
|
|  | [setHeight(int height)](#setHeight-int-) | Imposta l'altezza dell'anteprima della pagina. |
|
|  | [getDpi()](#getDpi--) | Ottiene un dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Imposta un dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Ottiene un array di numeri di pagina per generare le anteprime. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Imposta un array di numeri di pagina per generare le anteprime. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Ottiene il formato dell'immagine di anteprima. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Imposta il formato dell'immagine di anteprima. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Ottiene un'istanza del delegato di creazione dello stream della pagina. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Imposta un'istanza del delegato di creazione dello stream della pagina. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Ottiene un'istanza del delegato di completamento dell'anteprima della pagina. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Imposta un'istanza del delegato di completamento dell'anteprima della pagina. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Ottiene un'istanza del delegato di informazioni di rendering dell'anteprima della pagina. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Imposta un'istanza del delegato di informazioni di rendering dell'anteprima della pagina. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Inizializza una nuova istanza della classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) causando la chiusura del flusso di output.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Crea uno stream per una specifica anteprima della pagina. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Inizializza una nuova istanza della classe [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) facendo restituire il flusso di output al client per un uso successivo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Crea uno stream per una specifica anteprima della pagina |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Notifica che la generazione dell'anteprima della pagina è completata e ottiene lo stream di output. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Restituisce la larghezza dell'anteprima della pagina.


**Returns:**
int - La larghezza della pagina.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Imposta la larghezza dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | width | int | La larghezza della pagina. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Ottiene l'altezza dell'anteprima della pagina.


**Returns:**
int - L'altezza della pagina.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Imposta l'altezza dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | height | int | L'altezza della pagina. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Ottiene un dpi.


**Returns:**
int - Un valore intero che rappresenta un dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Imposta un dpi.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dpi | int | Il dpi. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Ottiene un array di numeri di pagina per generare le anteprime.


**Returns:**
int[] - Una collezione di numeri di pagina.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Imposta un array di numeri di pagina per generare le anteprime.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageNumbers | int[] | Una collezione di numeri di pagina. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Ottiene il formato dell'immagine di anteprima.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Imposta il formato dell'immagine di anteprima.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Il formato di anteprima. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Ottiene un'istanza del delegato di creazione dello stream della pagina.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Imposta un'istanza del delegato di creazione dello stream della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Il delegato di creazione del flusso di pagina. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Ottiene un'istanza del delegato di completamento dell'anteprima della pagina.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Imposta un'istanza del delegato di completamento dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Il delegato di completamento dell'anteprima della pagina. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Ottiene un'istanza del delegato di informazioni di rendering dell'anteprima della pagina.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Imposta un'istanza del delegato di informazioni di rendering dell'anteprima della pagina.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Il delegato di informazioni di rendering dell'anteprima della pagina. |
|

