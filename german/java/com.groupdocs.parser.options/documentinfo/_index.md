---
title: "DocumentInfo"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Dokumentinformationen dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Stellt die Dokumentinformationen dar.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileType()](#getFileType--) | Liefert den Dokumenttyp. |
|
|  | [getPageCount()](#getPageCount--) | Ermittelt die Gesamtzahl der Dokumentseiten. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Ermittelt die Gesamtzahl der rohen Dokumentseiten. |
|
|  | [getSize()](#getSize--) | Liefert die Größe des Dokuments in Bytes. |
|
|  | [getPages()](#getPages--) | Ermittelt die Informationen zu Seiten, wie den Index und die Seitengröße. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Liefert den Dokumenttyp.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Ermittelt die Gesamtzahl der Dokumentseiten.


**Returns:**
int - Ein ganzzahliger Wert, der die Gesamtzahl der Seiten darstellt.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Ermittelt die Gesamtzahl der rohen Dokumentseiten.

Verwenden Sie die Eigenschaft [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) anstelle der Eigenschaft [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) für die Extraktion von Rohtext.
Einige Dokumente haben unterschiedliche Seitenzahlen im genauen und im Rohtext‑Extraktionsmodus.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Ein ganzzahliger Wert, der die Gesamtzahl der rohen Seiten darstellt.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Liefert die Größe des Dokuments in Bytes.


**Returns:**
long - Ein ganzzahliger Wert, der die Größe des Dokuments in Bytes darstellt.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Ermittelt die Informationen zu Seiten, wie den Index und die Seitengröße.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Eine Sammlung von Instanzen der Klasse [PageInfo](../../com.groupdocs.parser.options/pageinfo).

