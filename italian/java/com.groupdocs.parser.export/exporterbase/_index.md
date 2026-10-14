---
title: "ExporterBase"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce la classe base per la funzionalità di esportazione dei dati."
type: docs
weight: 10
url: /it/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Fornisce la classe base per la funzionalità di esportazione dei dati.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Esporta la raccolta di metadati nello stream. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Esporta la raccolta di metadati nel file. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Esporta le informazioni del documento nello stream. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Esporta le informazioni del documento nel file. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Esporta la raccolta di aree di testo nello stream. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Esporta la raccolta di aree di testo nel file. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Esporta la raccolta di tabelle nello stream. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Esporta la raccolta di tabelle nel file. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Esporta la raccolta di codici a barre nello stream. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Esporta la raccolta di codici a barre nel file. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Esporta i dati del documento nello stream. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Esporta i dati del documento nel file. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Esporta la raccolta di metadati nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | metadati | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La raccolta di metadati. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Esporta la raccolta di metadati nel file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | metadati | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La raccolta di metadati. |
|
|  | fileName | java.lang.String | Il percorso completo del file di output. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Esporta le informazioni del documento nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Le informazioni del documento. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Esporta le informazioni del documento nel file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Le informazioni del documento. |
|
|  | fileName | java.lang.String | Il percorso completo del file di output. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Esporta la raccolta di aree di testo nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La raccolta delle aree di testo. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Esporta la raccolta di aree di testo nel file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La raccolta delle aree di testo. |
|
|  | fileName | java.lang.String | Il percorso completo del file di output. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Esporta la raccolta di tabelle nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La raccolta delle tabelle. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Esporta la raccolta di tabelle nel file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La raccolta delle tabelle. |
|
|  | fileName | java.lang.String | Il percorso completo del file di output. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Esporta la raccolta di codici a barre nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La raccolta dei codici a barre. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Esporta la raccolta di codici a barre nel file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La raccolta dei codici a barre. |
|
|  | fileName | java.lang.String | Il percorso completo del file di output. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Esporta i dati del documento nello stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dati del documento. |
|
|  | outputStream | java.io.OutputStream | Il flusso di output. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Esporta i dati del documento nel file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Dati del documento. |
|
|  | fileName | java.lang.String | Il percorso completo del file di output. |
|

