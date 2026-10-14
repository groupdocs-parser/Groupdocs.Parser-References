---
title: "XmlExporter"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الوظيفة لتصدير البيانات بتنسيق XML."
type: docs
weight: 11
url: /ar/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

يوفر الوظيفة لتصدير البيانات بتنسيق XML.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | ينشئ مثلاً جديداً من الفئة [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | يصدّر مجموعة البيانات الوصفية إلى الدفق. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | يصدّر معلومات المستند إلى الدفق. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | يصدّر مجموعة مناطق النص إلى الدفق. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | يصدّر مجموعة الجداول إلى الدفق. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | يصدّر مجموعة الباركود إلى الدفق. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | يصدّر بيانات المستند إلى الدفق. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


ينشئ مثلاً جديداً من الفئة [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


يصدّر مجموعة البيانات الوصفية إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | البيانات الوصفية | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | مجموعة البيانات الوصفية. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


يصدّر معلومات المستند إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | معلومات المستند. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


يصدّر مجموعة مناطق النص إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | مجموعة مناطق النص. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


يصدّر مجموعة الجداول إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea} | مجموعة الجداول. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


يصدّر مجموعة الباركود إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea} | مجموعة الباركود. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


يصدّر بيانات المستند إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | بيانات المستند. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

