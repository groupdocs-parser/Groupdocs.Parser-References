---
title: "DocumentInfo"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Vertegenwoordigt de documentinformatie."
type: docs
weight: 11
url: /nl/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Vertegenwoordigt de documentinformatie.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileType()](#getFileType--) | Haalt het documenttype op. |
|
|  | [getPageCount()](#getPageCount--) | Haalt het totale aantal documentpagina's op. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Haalt het totale aantal ruwe documentpagina's op. |
|
|  | [getSize()](#getSize--) | Haalt de grootte van het document op in bytes. |
|
|  | [getPages()](#getPages--) | Haalt de informatie over pagina's op, zoals de index en paginagrootte. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Haalt het documenttype op.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Haalt het totale aantal documentpagina's op.


**Returns:**
int - Een geheel getal dat het totale aantal pagina's weergeeft.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Haalt het totale aantal ruwe documentpagina's op.

Gebruik de eigenschap [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) in plaats van de eigenschap [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) voor ruwe tekstelextractie.
Sommige documenten hebben verschillende paginanummers in de nauwkeurige en ruwe tekstelextractiemodi.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Een geheel getal dat het totale aantal ruwe pagina's weergeeft.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Haalt de grootte van het document op in bytes.


**Returns:**
long - Een gehele waarde die de grootte van het document in bytes vertegenwoordigt.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Haalt de informatie over pagina's op, zoals de index en paginagrootte.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Een collectie met instanties van de klasse [PageInfo](../../com.groupdocs.parser.options/pageinfo).

