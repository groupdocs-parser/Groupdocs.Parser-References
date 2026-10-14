---
title: "ExporterBase"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供数据导出功能的基类。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

提供数据导出功能的基类。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | 将元数据集合导出到流中。 |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | 将元数据集合导出到文件中。 |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | 将文档信息导出到流中。 |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | 将文档信息导出到文件中。 |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | 将文本区域集合导出到流中。 |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | 将文本区域集合导出到文件中。 |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | 将表格集合导出到流中。 |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | 将表格集合导出到文件中。 |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | 将条形码集合导出到流中。 |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | 将条形码集合导出到文件中。 |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | 将文档数据导出到流中。 |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | 将文档数据导出到文件中。 |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


将元数据集合导出到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 元数据 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 元数据的集合。 |
|
|  | outputStream | java.io.OutputStream | 输出流。 |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


将元数据集合导出到文件中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 元数据 | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | 元数据的集合。 |
|
|  | fileName | java.lang.String | 输出文件的完整路径。 |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


将文档信息导出到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 文档信息。 |
|
|  | outputStream | java.io.OutputStream | 输出流。 |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


将文档信息导出到文件中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 文档信息。 |
|
|  | fileName | java.lang.String | 输出文件的完整路径。 |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


将文本区域集合导出到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 文本区域的集合。 |
|
|  | outputStream | java.io.OutputStream | 输出流。 |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


将文本区域集合导出到文件中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 文本区域集合。 |
|
|  | fileName | java.lang.String | 输出文件的完整路径。 |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


将表格集合导出到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 表格 | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | 表格的集合。 |
|
|  | outputStream | java.io.OutputStream | 输出流。 |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


将表格集合导出到文件中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 表格 | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | 表格的集合。 |
|
|  | fileName | java.lang.String | 输出文件的完整路径。 |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


将条形码集合导出到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 条形码 | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | 条形码的集合。 |
|
|  | outputStream | java.io.OutputStream | 输出流。 |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


将条形码集合导出到文件中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 条形码 | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | 条形码的集合。 |
|
|  | fileName | java.lang.String | 输出文件的完整路径。 |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


将文档数据导出到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 文档数据。 |
|
|  | outputStream | java.io.OutputStream | 输出流。 |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


将文档数据导出到文件中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 文档数据。 |
|
|  | fileName | java.lang.String | 输出文件的完整路径。 |
|

