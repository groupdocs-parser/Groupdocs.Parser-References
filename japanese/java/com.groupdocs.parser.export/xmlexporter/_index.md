---
title: "XmlExporter"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "データを XML 形式でエクスポートする機能を提供します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

データを XML 形式でエクスポートする機能を提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | 新しい [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | メタデータのコレクションをストリームにエクスポートします。 |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | ドキュメント情報をストリームにエクスポートします。 |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | テキスト領域のコレクションをストリームにエクスポートします。 |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | テーブルのコレクションをストリームにエクスポートします。 |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | バーコードのコレクションをストリームにエクスポートします。 |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | ドキュメントデータをストリームにエクスポートします。 |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


新しい [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) クラスのインスタンスを初期化します。


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


メタデータのコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | メタデータのコレクションです。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


ドキュメント情報をストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | 文書情報。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


テキスト領域のコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | テキスト領域のコレクション。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


テーブルのコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | テーブルのコレクション。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


バーコードのコレクションをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | バーコードのコレクション。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


ドキュメントデータをストリームにエクスポートします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | 文書データ。 |
|
|  | outputStream | java.io.OutputStream | 出力ストリーム。 |
|

