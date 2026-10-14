---
title: "XmlExporter"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Funktionalität zum Exportieren von Daten im XML-Format bereit."
type: docs
weight: 11
url: /de/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Stellt die Funktionalität zum Exportieren von Daten im XML-Format bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Initialisiert eine neue Instanz der [XmlExporter](../../com.groupdocs.parser.export/xmlexporter)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exportiert die Sammlung von Metadaten in den Stream. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exportiert die Dokumentinformationen in den Stream. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exportiert die Sammlung von Textbereichen in den Stream. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exportiert die Sammlung von Tabellen in den Stream. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exportiert die Sammlung von Barcodes in den Stream. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exportiert Dokumentdaten in den Stream. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Initialisiert eine neue Instanz der [XmlExporter](../../com.groupdocs.parser.export/xmlexporter)-Klasse.


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exportiert die Sammlung von Metadaten in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Metadaten | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Die Sammlung von Metadaten. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exportiert die Dokumentinformationen in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Die Dokumentinformationen. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exportiert die Sammlung von Textbereichen in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Die Sammlung der Textbereiche. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exportiert die Sammlung von Tabellen in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Tabellen | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Die Sammlung von Tabellen. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exportiert die Sammlung von Barcodes in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Strichcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Die Sammlung von Strichcodes. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exportiert Dokumentdaten in den Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dokumentdaten. |
|
|  | outputStream | java.io.OutputStream | Der Ausgabestream. |
|

