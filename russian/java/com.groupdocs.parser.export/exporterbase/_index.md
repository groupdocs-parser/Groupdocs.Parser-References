---
title: "ExporterBase"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет базовый класс для функциональности экспорта данных."
type: docs
weight: 10
url: /ru/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Предоставляет базовый класс для функциональности экспорта данных.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Экспортирует коллекцию метаданных в поток. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Экспортирует коллекцию метаданных в файл. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Экспортирует информацию о документе в поток. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Экспортирует информацию о документе в файл. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Экспортирует коллекцию текстовых областей в поток. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Экспортирует коллекцию текстовых областей в файл. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Экспортирует коллекцию таблиц в поток. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Экспортирует коллекцию таблиц в файл. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Экспортирует коллекцию штрих-кодов в поток. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Экспортирует коллекцию штрих-кодов в файл. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Экспортирует данные документа в поток. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Экспортирует данные документа в файл. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Экспортирует коллекцию метаданных в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Коллекция метаданных. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Экспортирует коллекцию метаданных в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Коллекция метаданных. |
|
|  | fileName | java.lang.String | Полный путь к файлу вывода. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Экспортирует информацию о документе в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Информация о документе. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Экспортирует информацию о документе в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Информация о документе. |
|
|  | fileName | java.lang.String | Полный путь к файлу вывода. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Экспортирует коллекцию текстовых областей в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Коллекция текстовых областей. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Экспортирует коллекцию текстовых областей в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Коллекция текстовых областей. |
|
|  | fileName | java.lang.String | Полный путь к файлу вывода. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Экспортирует коллекцию таблиц в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Коллекция таблиц. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Экспортирует коллекцию таблиц в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Коллекция таблиц. |
|
|  | fileName | java.lang.String | Полный путь к файлу вывода. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Экспортирует коллекцию штрих-кодов в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Коллекция штрихкодов. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Экспортирует коллекцию штрих-кодов в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Коллекция штрихкодов. |
|
|  | fileName | java.lang.String | Полный путь к файлу вывода. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Экспортирует данные документа в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Данные документа. |
|
|  | outputStream | java.io.OutputStream | Поток вывода. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Экспортирует данные документа в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Данные документа. |
|
|  | fileName | java.lang.String | Полный путь к файлу вывода. |
|

