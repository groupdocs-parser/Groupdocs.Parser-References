---
title: "DocumentInfo"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información del documento."
type: docs
weight: 11
url: /es/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Representa la información del documento.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtiene el tipo de documento. |
|
|  | [getPageCount()](#getPageCount--) | Obtiene el número total de páginas del documento. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Obtiene el número total de páginas sin procesar del documento. |
|
|  | [getSize()](#getSize--) | Obtiene el tamaño del documento en bytes. |
|
|  | [getPages()](#getPages--) | Obtiene la información sobre las páginas, como el índice y el tamaño de la página. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Obtiene el tipo de documento.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Obtiene el número total de páginas del documento.


**Returns:**
int - Un valor entero que representa el número total de páginas.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Obtiene el número total de páginas sin procesar del documento.

Utilice la propiedad [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) en lugar de la propiedad [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) para la extracción de texto sin procesar.
Algunos documentos tienen diferentes números de página en los modos de extracción de texto preciso y sin procesar.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Un valor entero que representa el número total de páginas sin procesar.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Obtiene el tamaño del documento en bytes.


**Returns:**
long - Un valor entero que representa el tamaño del documento en bytes.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Obtiene la información sobre las páginas, como el índice y el tamaño de la página.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Una colección con instancias de clases [PageInfo](../../com.groupdocs.parser.options/pageinfo).

