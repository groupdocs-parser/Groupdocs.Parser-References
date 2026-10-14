---
title: "XmlExporter"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit la fonctionnalité d'exportation de données au format XML."
type: docs
weight: 11
url: /fr/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Fournit la fonctionnalité d'exportation de données au format XML.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Initialise une nouvelle instance de la classe [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exporte la collection de métadonnées vers le flux. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exporte les informations du document vers le flux. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exporte la collection de zones de texte vers le flux. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exporte la collection de tableaux vers le flux. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exporte la collection de codes-barres vers le flux. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exporte les données du document vers le flux. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Initialise une nouvelle instance de la classe [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exporte la collection de métadonnées vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | métadonnées | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collection de métadonnées. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exporte les informations du document vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Les informations du document. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exporte la collection de zones de texte vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La collection des zones de texte. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exporte la collection de tableaux vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La collection de tables. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exporte la collection de codes-barres vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | codes-barres | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La collection de codes-barres. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exporte les données du document vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Données du document. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

