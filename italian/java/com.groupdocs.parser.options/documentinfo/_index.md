---
title: "DocumentInfo"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni del documento."
type: docs
weight: 11
url: /it/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Rappresenta le informazioni del documento.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileType()](#getFileType--) | Restituisce il tipo di documento. |
|
|  | [getPageCount()](#getPageCount--) | Restituisce il numero totale di pagine del documento. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Restituisce il numero totale di pagine grezze del documento. |
|
|  | [getSize()](#getSize--) | Restituisce la dimensione del documento in byte. |
|
|  | [getPages()](#getPages--) | Restituisce le informazioni sulle pagine, come l'indice e le dimensioni della pagina. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Restituisce il tipo di documento.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Restituisce il numero totale di pagine del documento.


**Returns:**
int - Un valore intero che rappresenta il numero totale di pagine.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Restituisce il numero totale di pagine grezze del documento.

Usa la proprietà [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) invece della proprietà [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) per l'estrazione del testo grezzo.
Alcuni documenti hanno numeri di pagina diversi nelle modalità di estrazione del testo accurata e grezza.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Un valore intero che rappresenta il numero totale di pagine grezze.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Restituisce la dimensione del documento in byte.


**Returns:**
long - Un valore intero che rappresenta la dimensione del documento in byte.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Restituisce le informazioni sulle pagine, come l'indice e le dimensioni della pagina.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Una collezione con istanze delle classi [PageInfo](../../com.groupdocs.parser.options/pageinfo).

