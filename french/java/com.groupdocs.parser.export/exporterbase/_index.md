---
title: "ExporterBase"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit la classe de base pour la fonctionnalité d'exportation de données."
type: docs
weight: 10
url: /fr/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Fournit la classe de base pour la fonctionnalité d'exportation de données.

## Constructors

| Constructor | Description |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Exporte la collection de métadonnées vers le flux. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Exporte la collection de métadonnées vers le fichier. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Exporte les informations du document vers le flux. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Exporte les informations du document vers le fichier. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Exporte la collection de zones de texte vers le flux. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Exporte la collection de zones de texte vers le fichier. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Exporte la collection de tableaux vers le flux. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Exporte la collection de tableaux vers le fichier. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Exporte la collection de codes-barres vers le flux. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Exporte la collection de codes-barres vers le fichier. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Exporte les données du document vers le flux. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Exporte les données du document vers le fichier. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Exporte la collection de métadonnées vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | métadonnées | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collection de métadonnées. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Exporte la collection de métadonnées vers le fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | métadonnées | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collection de métadonnées. |
|
|  | fileName | java.lang.String | Le chemin complet vers le fichier de sortie. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Exporte les informations du document vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Les informations du document. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Exporte les informations du document vers le fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Les informations du document. |
|
|  | fileName | java.lang.String | Le chemin complet vers le fichier de sortie. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Exporte la collection de zones de texte vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La collection des zones de texte. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Exporte la collection de zones de texte vers le fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La collection des zones de texte. |
|
|  | fileName | java.lang.String | Le chemin complet vers le fichier de sortie. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Exporte la collection de tableaux vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La collection de tables. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Exporte la collection de tableaux vers le fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | La collection de tables. |
|
|  | fileName | java.lang.String | Le chemin complet vers le fichier de sortie. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Exporte la collection de codes-barres vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | codes-barres | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La collection de codes-barres. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Exporte la collection de codes-barres vers le fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | codes-barres | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | La collection de codes-barres. |
|
|  | fileName | java.lang.String | Le chemin complet vers le fichier de sortie. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Exporte les données du document vers le flux.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Données du document. |
|
|  | outputStream | java.io.OutputStream | Le flux de sortie. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Exporte les données du document vers le fichier.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Données du document. |
|
|  | fileName | java.lang.String | Le chemin complet vers le fichier de sortie. |
|

