---
title: ExporterBase
second_title: GroupDocs.Parser for Java API Reference
description: Provides the base class for the data export functionality.
type: docs
weight: 10
url: /java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Provides the base class for the data export functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Methods

| Method | Description |
| --- | --- |
| [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exports the collection of metadata to the stream. |
| [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Exports the collection of metadata to the file. |
| [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exports the document information to the stream. |
| [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Exports the document information to the file. |
| [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exports the collection of text areas to the stream. |
| [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Exports the collection of text areas to the file. |
| [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exports the collection of tables to the stream. |
| [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Exports the collection of tables to the file. |
| [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exports the collection of barcodes to the stream. |
| [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Exports the collection of barcodes to the file. |
| [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exports document data to the stream. |
| [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Exports document data to the file. |
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exports the collection of metadata to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | The collection of metadata. |
| outputStream | java.io.OutputStream | The output stream. |

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Exports the collection of metadata to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | The collection of metadata. |
| fileName | java.lang.String | The full path to the output file. |

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exports the document information to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | The document information. |
| outputStream | java.io.OutputStream | The output stream. |

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Exports the document information to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | The document information. |
| fileName | java.lang.String | The full path to the output file. |

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exports the collection of text areas to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | The collection of the text areas. |
| outputStream | java.io.OutputStream | The output stream. |

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Exports the collection of text areas to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | The collection of text areas. |
| fileName | java.lang.String | The full path to the output file. |

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exports the collection of tables to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | The collection of tables. |
| outputStream | java.io.OutputStream | The output stream. |

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Exports the collection of tables to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | The collection of tables. |
| fileName | java.lang.String | The full path to the output file. |

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exports the collection of barcodes to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | The collection of barcodes. |
| outputStream | java.io.OutputStream | The output stream. |

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Exports the collection of barcodes to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | The collection of barcodes. |
| fileName | java.lang.String | The full path to the output file. |

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exports document data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Document data. |
| outputStream | java.io.OutputStream | The output stream. |

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Exports document data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Document data. |
| fileName | java.lang.String | The full path to the output file. |

