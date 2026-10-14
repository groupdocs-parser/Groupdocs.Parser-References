---
title: "ExporterBase"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الفئة الأساسية لوظيفة تصدير البيانات."
type: docs
weight: 10
url: /ar/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

يوفر الفئة الأساسية لوظيفة تصدير البيانات.

## البناؤات

| البناء | الوصف |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | يصدّر مجموعة البيانات الوصفية إلى الدفق. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | يصدّر مجموعة البيانات الوصفية إلى الملف. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | يصدّر معلومات المستند إلى الدفق. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | يصدّر معلومات المستند إلى الملف. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | يصدّر مجموعة مناطق النص إلى الدفق. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | يصدّر مجموعة مناطق النص إلى الملف. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | يصدّر مجموعة الجداول إلى الدفق. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | يصدّر مجموعة الجداول إلى الملف. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | يصدّر مجموعة الباركود إلى الدفق. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | يصدّر مجموعة الباركود إلى الملف. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | يصدّر بيانات المستند إلى الدفق. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | يصدّر بيانات المستند إلى الملف. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


يصدّر مجموعة البيانات الوصفية إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | البيانات الوصفية | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | مجموعة البيانات الوصفية. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


يصدّر مجموعة البيانات الوصفية إلى الملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | البيانات الوصفية | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | مجموعة البيانات الوصفية. |
|
|  | fileName | java.lang.String | المسار الكامل إلى ملف الإخراج. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


يصدّر معلومات المستند إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | معلومات المستند. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


يصدّر معلومات المستند إلى الملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | معلومات المستند. |
|
|  | fileName | java.lang.String | المسار الكامل إلى ملف الإخراج. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


يصدّر مجموعة مناطق النص إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | مجموعة مناطق النص. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


يصدّر مجموعة مناطق النص إلى الملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | مجموعة مناطق النص. |
|
|  | fileName | java.lang.String | المسار الكامل إلى ملف الإخراج. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


يصدّر مجموعة الجداول إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea} | مجموعة الجداول. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


يصدّر مجموعة الجداول إلى الملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea} | مجموعة الجداول. |
|
|  | fileName | java.lang.String | المسار الكامل إلى ملف الإخراج. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


يصدّر مجموعة الباركود إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea} | مجموعة الباركود. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


يصدّر مجموعة الباركود إلى الملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea} | مجموعة الباركود. |
|
|  | fileName | java.lang.String | المسار الكامل إلى ملف الإخراج. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


يصدّر بيانات المستند إلى الدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | بيانات المستند. |
|
|  | outputStream | java.io.OutputStream | دفق الإخراج. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


يصدّر بيانات المستند إلى الملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | بيانات المستند. |
|
|  | fileName | java.lang.String | المسار الكامل إلى ملف الإخراج. |
|

