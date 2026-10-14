---
title: "XmlExporter"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller funktionaliteten för att exportera data i XML-format."
type: docs
weight: 11
url: /sv/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Tillhandahåller funktionaliteten för att exportera data i XML-format.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Initierar en ny instans av klassen [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exporterar samlingen av metadata till strömmen. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exporterar dokumentinformationen till strömmen. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exporterar samlingen av textområden till strömmen. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exporterar samlingen av tabeller till strömmen. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exporterar samlingen av streckkoder till strömmen. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exporterar dokumentdata till strömmen. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Initierar en ny instans av klassen [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exporterar samlingen av metadata till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Samlingen av metadata. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exporterar dokumentinformationen till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Dokumentinformationen. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exporterar samlingen av textområden till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Samlingen av textområdena. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exporterar samlingen av tabeller till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Samlingen av tabeller. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exporterar samlingen av streckkoder till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Samlingen av streckkoder. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exporterar dokumentdata till strömmen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dokumentdata. |
|
|  | outputStream | java.io.OutputStream | Utdataströmmen. |
|

