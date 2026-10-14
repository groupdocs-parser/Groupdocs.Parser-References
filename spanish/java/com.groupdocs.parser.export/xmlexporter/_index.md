---
title: "XmlExporter"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona la funcionalidad para exportar datos en formato XML."
type: docs
weight: 11
url: /es/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Proporciona la funcionalidad para exportar datos en formato XML.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Inicializa una nueva instancia de la clase [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exporta la colección de metadatos al flujo. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exporta la información del documento al flujo. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exporta la colección de áreas de texto al flujo. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exporta la colección de tablas al flujo. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exporta la colección de códigos de barras al flujo. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exporta los datos del documento al flujo. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Inicializa una nueva instancia de la clase [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exporta la colección de metadatos al flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La colección de metadatos. |
|
|  | outputStream | java.io.OutputStream | El flujo de salida. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exporta la información del documento al flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | La información del documento. |
|
|  | outputStream | java.io.OutputStream | El flujo de salida. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exporta la colección de áreas de texto al flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La colección de las áreas de texto. |
|
|  | outputStream | java.io.OutputStream | El flujo de salida. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exporta la colección de tablas al flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La colección de tablas. |
|
|  | outputStream | java.io.OutputStream | El flujo de salida. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exporta la colección de códigos de barras al flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La colección de códigos de barras. |
|
|  | outputStream | java.io.OutputStream | El flujo de salida. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exporta los datos del documento al flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Datos del documento. |
|
|  | outputStream | java.io.OutputStream | El flujo de salida. |
|

