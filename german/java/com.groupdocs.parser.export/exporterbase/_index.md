---
title: "ExporterBase"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Basisklasse für die Datenexportfunktionalität bereit."
type: docs
weight: 10
url: /de/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Stellt die Basisklasse für die Datenexportfunktionalität bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exportiert die Sammlung von Metadaten in den Stream. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Exportiert die Sammlung von Metadaten in die Datei. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exportiert die Dokumentinformationen in den Stream. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Exportiert die Dokumentinformationen in die Datei. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exportiert die Sammlung von Textbereichen in den Stream. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Exportiert die Sammlung von Textbereichen in die Datei. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exportiert die Sammlung von Tabellen in den Stream. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Exportiert die Sammlung von Tabellen in die Datei. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exportiert die Sammlung von Barcodes in den Stream. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Exportiert die Sammlung von Barcodes in die Datei. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exportiert Dokumentdaten in den Stream. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Exportiert Dokumentdaten in die Datei. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exportiert die Sammlung von Metadaten in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Metadaten | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Die Sammlung von Metadaten. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Exportiert die Sammlung von Metadaten in die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Metadaten | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Die Sammlung von Metadaten. |
|
|  | fileName | java.lang.String | Der vollständige Pfad zur Ausgabedatei. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exportiert die Dokumentinformationen in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Die Dokumentinformationen. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Exportiert die Dokumentinformationen in die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Die Dokumentinformationen. |
|
|  | fileName | java.lang.String | Der vollständige Pfad zur Ausgabedatei. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exportiert die Sammlung von Textbereichen in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Die Sammlung der Textbereiche. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Exportiert die Sammlung von Textbereichen in die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Die Sammlung von Textbereichen. |
|
|  | fileName | java.lang.String | Der vollständige Pfad zur Ausgabedatei. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exportiert die Sammlung von Tabellen in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Tabellen | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Die Sammlung von Tabellen. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Exportiert die Sammlung von Tabellen in die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Tabellen | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Die Sammlung von Tabellen. |
|
|  | fileName | java.lang.String | Der vollständige Pfad zur Ausgabedatei. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exportiert die Sammlung von Barcodes in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Strichcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Die Sammlung von Strichcodes. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Exportiert die Sammlung von Barcodes in die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Strichcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Die Sammlung von Strichcodes. |
|
|  | fileName | java.lang.String | Der vollständige Pfad zur Ausgabedatei. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exportiert Dokumentdaten in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dokumentdaten. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Exportiert Dokumentdaten in die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dokumentdaten. |
|
|  | fileName | java.lang.String | Der vollständige Pfad zur Ausgabedatei. |
|

