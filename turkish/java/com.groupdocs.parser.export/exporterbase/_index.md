---
title: "ExporterBase"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Veri dışa aktarma işlevselliği için temel sınıfı sağlar."
type: docs
weight: 10
url: /tr/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Veri dışa aktarma işlevselliği için temel sınıfı sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Meta verilerin koleksiyonunu akışa dışa aktarır. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Meta verilerin koleksiyonunu dosyaya dışa aktarır. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Belge bilgisini akışa dışa aktarır. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Belge bilgisini dosyaya dışa aktarır. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Metin alanlarının koleksiyonunu akışa dışa aktarır. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Metin alanlarının koleksiyonunu dosyaya dışa aktarır. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Tabloların koleksiyonunu akışa dışa aktarır. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Tabloların koleksiyonunu dosyaya dışa aktarır. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Barkod koleksiyonunu akışa dışa aktarır. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Barkod koleksiyonunu dosyaya dışa aktarır. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Belge verilerini akışa dışa aktarır. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Belge verilerini dosyaya dışa aktarır. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Meta verilerin koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | meta veri | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Meta veri koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Meta verilerin koleksiyonunu dosyaya dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | meta veri | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Meta veri koleksiyonu. |
|
|  | fileName | java.lang.String | Çıktı dosyasının tam yolu. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Belge bilgisini akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Belge bilgileri. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Belge bilgisini dosyaya dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Belge bilgileri. |
|
|  | fileName | java.lang.String | Çıktı dosyasının tam yolu. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Metin alanlarının koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Metin alanlarının koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Metin alanlarının koleksiyonunu dosyaya dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Metin alanları koleksiyonu. |
|
|  | fileName | java.lang.String | Çıktı dosyasının tam yolu. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Tabloların koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Tabloların koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Tabloların koleksiyonunu dosyaya dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Tabloların koleksiyonu. |
|
|  | fileName | java.lang.String | Çıktı dosyasının tam yolu. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Barkod koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Barkodların koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Barkod koleksiyonunu dosyaya dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Barkodların koleksiyonu. |
|
|  | fileName | java.lang.String | Çıktı dosyasının tam yolu. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Belge verilerini akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Belge verileri. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Belge verilerini dosyaya dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Belge verileri. |
|
|  | fileName | java.lang.String | Çıktı dosyasının tam yolu. |
|

