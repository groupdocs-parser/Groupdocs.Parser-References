---
title: "XmlExporter"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет возможность экспорта данных в формате XML."
type: docs
weight: 11
url: /ru/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Предоставляет возможность экспорта данных в формате XML.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Инициализирует новый экземпляр класса [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Экспортирует коллекцию метаданных в поток. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Экспортирует информацию о документе в поток. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Экспортирует коллекцию текстовых областей в поток. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Экспортирует коллекцию таблиц в поток. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Экспортирует коллекцию штрих-кодов в поток. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Экспортирует данные документа в поток. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Инициализирует новый экземпляр класса [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Экспортирует коллекцию метаданных в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Коллекция метаданных. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Экспортирует информацию о документе в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Информация о документе. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Экспортирует коллекцию текстовых областей в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Коллекция текстовых областей. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Экспортирует коллекцию таблиц в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Коллекция таблиц. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Экспортирует коллекцию штрих-кодов в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Коллекция штрихкодов. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Экспортирует данные документа в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Данные документа. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

