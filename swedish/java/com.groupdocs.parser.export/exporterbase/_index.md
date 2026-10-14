---
title: "ExporterBase"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller basklassen för dataexportfunktionaliteten."
type: docs
weight: 10
url: /sv/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Tillhandahåller basklassen för dataexportfunktionaliteten.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exporterar samlingen av metadata till strömmen. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Exporterar samlingen av metadata till filen. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exporterar dokumentinformationen till strömmen. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Exporterar dokumentinformationen till filen. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exporterar samlingen av textområden till strömmen. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Exporterar samlingen av textområden till filen. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exporterar samlingen av tabeller till strömmen. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Exporterar samlingen av tabeller till filen. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exporterar samlingen av streckkoder till strömmen. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Exporterar samlingen av streckkoder till filen. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exporterar dokumentdata till strömmen. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Exporterar dokumentdata till filen. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exporterar samlingen av metadata till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Samlingen av metadata. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Exporterar samlingen av metadata till filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Samlingen av metadata. |
|
|  | fileName | java.lang.String | Den fullständiga sökvägen till utdatafilen. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exporterar dokumentinformationen till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Dokumentinformationen. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Exporterar dokumentinformationen till filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Dokumentinformationen. |
|
|  | fileName | java.lang.String | Den fullständiga sökvägen till utdatafilen. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exporterar samlingen av textområden till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Samlingen av textområdena. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Exporterar samlingen av textområden till filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Samlingen av textområden. |
|
|  | fileName | java.lang.String | Den fullständiga sökvägen till utdatafilen. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exporterar samlingen av tabeller till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Samlingen av tabeller. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Exporterar samlingen av tabeller till filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Samlingen av tabeller. |
|
|  | fileName | java.lang.String | Den fullständiga sökvägen till utdatafilen. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exporterar samlingen av streckkoder till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Samlingen av streckkoder. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Exporterar samlingen av streckkoder till filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Samlingen av streckkoder. |
|
|  | fileName | java.lang.String | Den fullständiga sökvägen till utdatafilen. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exporterar dokumentdata till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dokumentdata. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Exporterar dokumentdata till filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dokumentdata. |
|
|  | fileName | java.lang.String | Den fullständiga sökvägen till utdatafilen. |
|

