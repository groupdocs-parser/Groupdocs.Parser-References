---
title: "ExporterBase"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "データエクスポート機能の基底クラスを提供します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

データエクスポート機能の基底クラスを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | メタデータのコレクションをストリームにエクスポートします。 |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | メタデータのコレクションをファイルにエクスポートします。 |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | ドキュメント情報をストリームにエクスポートします。 |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | ドキュメント情報をファイルにエクスポートします。 |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | テキスト領域のコレクションをストリームにエクスポートします。 |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | テキスト領域のコレクションをファイルにエクスポートします。 |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | テーブルのコレクションをストリームにエクスポートします。 |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | テーブルのコレクションをファイルにエクスポートします。 |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | バーコードのコレクションをストリームにエクスポートします。 |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | バーコードのコレクションをファイルにエクスポートします。 |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | ドキュメントデータをストリームにエクスポートします。 |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | ドキュメントデータをファイルにエクスポートします。 |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


メタデータのコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | メタデータのコレクションです。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


メタデータのコレクションをファイルにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | メタデータのコレクションです。 |
|
|  | fileName | java.lang.String | 出力ファイルの完全パス。 |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


ドキュメント情報をストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 文書情報。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


ドキュメント情報をファイルにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 文書情報。 |
|
|  | fileName | java.lang.String | 出力ファイルの完全パス。 |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


テキスト領域のコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | テキスト領域のコレクション。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


テキスト領域のコレクションをファイルにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | テキスト領域のコレクション。 |
|
|  | fileName | java.lang.String | 出力ファイルの完全パス。 |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


テーブルのコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | テーブルのコレクション。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


テーブルのコレクションをファイルにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | テーブルのコレクション。 |
|
|  | fileName | java.lang.String | 出力ファイルの完全パス。 |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


バーコードのコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | バーコードのコレクション。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


バーコードのコレクションをファイルにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | バーコードのコレクション。 |
|
|  | fileName | java.lang.String | 出力ファイルの完全パス。 |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


ドキュメントデータをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 文書データ。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


ドキュメントデータをファイルにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 文書データ。 |
|
|  | fileName | java.lang.String | 出力ファイルの完全パス。 |
|

