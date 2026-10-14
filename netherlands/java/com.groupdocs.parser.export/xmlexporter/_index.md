---
title: "XmlExporter"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de functionaliteit om gegevens te exporteren in XML-formaat."
type: docs
weight: 11
url: /nl/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Biedt de functionaliteit om gegevens te exporteren in XML-formaat.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Initialiseert een nieuw exemplaar van de klasse [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exporteert de verzameling metadata naar de stream. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exporteert de documentinformatie naar de stream. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exporteert de verzameling tekstgebieden naar de stream. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exporteert de verzameling tabellen naar de stream. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exporteert de verzameling barcodes naar de stream. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exporteert documentgegevens naar de stream. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Initialiseert een nieuw exemplaar van de klasse [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exporteert de verzameling metadata naar de stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | De verzameling metadata. |
|
|  | outputStream | java.io.OutputStream | De uitvoerstream. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exporteert de documentinformatie naar de stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | De documentinformatie. |
|
|  | outputStream | java.io.OutputStream | De uitvoerstream. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exporteert de verzameling tekstgebieden naar de stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | De verzameling van de tekstgebieden. |
|
|  | outputStream | java.io.OutputStream | De uitvoerstream. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exporteert de verzameling tabellen naar de stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | De verzameling tabellen. |
|
|  | outputStream | java.io.OutputStream | De uitvoerstream. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exporteert de verzameling barcodes naar de stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | De verzameling barcodes. |
|
|  | outputStream | java.io.OutputStream | De uitvoerstream. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exporteert documentgegevens naar de stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Documentgegevens. |
|
|  | outputStream | java.io.OutputStream | De uitvoerstream. |
|

