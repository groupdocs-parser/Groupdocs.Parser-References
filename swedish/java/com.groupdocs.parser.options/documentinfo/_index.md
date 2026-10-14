---
title: "DocumentInfo"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar dokumentinformationen."
type: docs
weight: 11
url: /sv/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Representerar dokumentinformationen.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileType()](#getFileType--) | Hämtar dokumenttypen. |
|
|  | [getPageCount()](#getPageCount--) | Hämtar det totala antalet sidor i dokumentet. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Hämtar det totala antalet råa sidor i dokumentet. |
|
|  | [getSize()](#getSize--) | Hämtar storleken på dokumentet i byte. |
|
|  | [getPages()](#getPages--) | Hämtar information om sidor, såsom index och sidstorlek. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Hämtar dokumenttypen.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Hämtar det totala antalet sidor i dokumentet.


**Returns:**
int - Ett heltalsvärde som representerar det totala antalet sidor.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Hämtar det totala antalet råa sidor i dokumentet.

Använd egenskapen [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) istället för egenskapen [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) för råtextutvinning.
Vissa dokument har olika sidnummer i exakta och råa textutvinningslägen.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Ett heltalsvärde som representerar det totala antalet råa sidor.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Hämtar storleken på dokumentet i byte.


**Returns:**
long - Ett heltal som representerar storleken på dokumentet i byte.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Hämtar information om sidor, såsom index och sidstorlek.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - En samling med instanser av klasserna [PageInfo](../../com.groupdocs.parser.options/pageinfo).

