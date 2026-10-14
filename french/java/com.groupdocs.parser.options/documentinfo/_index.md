---
title: "DocumentInfo"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations du document."
type: docs
weight: 11
url: /fr/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Représente les informations du document.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtient le type de document. |
|
|  | [getPageCount()](#getPageCount--) | Obtient le nombre total de pages du document. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Obtient le nombre total de pages brutes du document. |
|
|  | [getSize()](#getSize--) | Obtient la taille du document en octets. |
|
|  | [getPages()](#getPages--) | Obtient les informations sur les pages telles que l'index et la taille de la page. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Obtient le type de document.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Obtient le nombre total de pages du document.


**Returns:**
int - Une valeur entière qui représente le nombre total de pages.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Obtient le nombre total de pages brutes du document.

Utilisez la propriété [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) au lieu de la propriété [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) pour l'extraction de texte brut.
Certains documents ont des numéros de page différents selon les modes d'extraction de texte précis et brut.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Une valeur entière qui représente le nombre total de pages brutes.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Obtient la taille du document en octets.


**Returns:**
long - Une valeur entière qui représente la taille du document en octets.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Obtient les informations sur les pages telles que l'index et la taille de la page.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Une collection contenant des instances des classes [PageInfo](../../com.groupdocs.parser.options/pageinfo).

