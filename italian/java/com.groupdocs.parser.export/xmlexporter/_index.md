---
title: "XmlExporter"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce la funzionalità per esportare i dati in formato XML."
type: docs
weight: 11
url: /it/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Fornisce la funzionalità per esportare i dati in formato XML.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Inizializza una nuova istanza della classe [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Esporta la raccolta di metadati nello stream. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Esporta le informazioni del documento nello stream. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Esporta la raccolta di aree di testo nello stream. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Esporta la raccolta di tabelle nello stream. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Esporta la raccolta di codici a barre nello stream. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Esporta i dati del documento nello stream. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Inizializza una nuova istanza della classe [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Esporta la raccolta di metadati nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | metadati | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La raccolta di metadati. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Esporta le informazioni del documento nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Le informazioni del documento. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Esporta la raccolta di aree di testo nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La raccolta delle aree di testo. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Esporta la raccolta di tabelle nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La raccolta delle tabelle. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Esporta la raccolta di codici a barre nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La raccolta dei codici a barre. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Esporta i dati del documento nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dati del documento. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

