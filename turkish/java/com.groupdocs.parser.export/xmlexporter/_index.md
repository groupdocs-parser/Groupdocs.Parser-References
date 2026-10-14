---
title: "XmlExporter"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Verileri XML formatında dışa aktarma işlevselliğini sağlar."
type: docs
weight: 11
url: /tr/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Verileri XML formatında dışa aktarma işlevselliğini sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Yeni bir [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Meta verilerin koleksiyonunu akışa dışa aktarır. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Belge bilgisini akışa dışa aktarır. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Metin alanlarının koleksiyonunu akışa dışa aktarır. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Tabloların koleksiyonunu akışa dışa aktarır. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Barkod koleksiyonunu akışa dışa aktarır. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Belge verilerini akışa dışa aktarır. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Yeni bir [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) sınıfının örneğini başlatır.


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Meta verilerin koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | meta veri | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Meta veri koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Belge bilgisini akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Belge bilgileri. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Metin alanlarının koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Metin alanlarının koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Tabloların koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Tabloların koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Barkod koleksiyonunu akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Barkodların koleksiyonu. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Belge verilerini akışa dışa aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Belge verileri. |
|
|  | outputStream | java.io.OutputStream | Çıktı akışı. |
|

