---
title: XmlExporter
second_title: GroupDocs.Parser for Java API Reference
description: Provides the functionality to export data in XML format.
type: docs
weight: 11
url: /java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Provides the functionality to export data in XML format.
## Constructors

| Constructor | Description |
| --- | --- |
| [XmlExporter()](#XmlExporter--) |  |
## Methods

| Method | Description |
| --- | --- |
| [exportMetadata(Iterable<MetadataItem> metadata, OutputStream stream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) |  |
| [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream stream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) |  |
| [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream stream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) |  |
| [exportTables(Iterable<PageTableArea> tables, OutputStream stream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) |  |
| [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream stream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) |  |
| [exportDocumentData(DocumentData documentData, OutputStream stream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) |  |
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream stream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream stream)
```


Exports the collection of metadata to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> |  |
| stream | java.io.OutputStream |  |

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream stream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream stream)
```


Exports the document information to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) |  |
| stream | java.io.OutputStream |  |

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream stream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream stream)
```


Exports the collection of text areas to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> |  |
| stream | java.io.OutputStream |  |

### exportTables(Iterable<PageTableArea> tables, OutputStream stream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream stream)
```


Exports the collection of tables to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> |  |
| stream | java.io.OutputStream |  |

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream stream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream stream)
```


Exports the collection of barcodes to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> |  |
| stream | java.io.OutputStream |  |

### exportDocumentData(DocumentData documentData, OutputStream stream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream stream)
```


Exports document data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) |  |
| stream | java.io.OutputStream |  |

