---
title: "エクスポート"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "メタデータのコレクションをストリームにエクスポートします。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

メタデータのコレクションをストリームにエクスポートします。

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| メタデータ | IEnumerable`1 | メタデータのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

メタデータのコレクションをファイルにエクスポートします。

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| メタデータ | IEnumerable`1 | メタデータのコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

ドキュメント情報をストリームにエクスポートします。

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 文書情報です。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

ドキュメント情報をファイルにエクスポートします。

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 文書情報です。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

テキスト領域のコレクションをストリームにエクスポートします。

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | テキスト領域のコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

テキスト領域のコレクションをファイルにエクスポートします。

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | テキスト領域のコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

テーブルのコレクションをストリームにエクスポートします。

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| tables | IEnumerable`1 | テーブルのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

テーブルのコレクションをファイルにエクスポートします。

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| tables | IEnumerable`1 | テーブルのコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

バーコードのコレクションをストリームにエクスポートします。

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| barcodes | IEnumerable`1 | バーコードのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

バーコードのコレクションをファイルにエクスポートします。

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| barcodes | IEnumerable`1 | バーコードのコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

ドキュメントデータをストリームにエクスポートします。

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentData | DocumentData | 文書データです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

ドキュメントデータをファイルにエクスポートします。

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentData | DocumentData | 文書データです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
