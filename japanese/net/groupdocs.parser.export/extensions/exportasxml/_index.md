---
title: "ExportAsXml"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "メタデータのコレクションをストリームに XML 形式でエクスポートします。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser.export/extensions/exportasxml/
---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasxml_4}

メタデータのコレクションをストリームに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| メタデータ | IEnumerable`1 | メタデータのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasxml_5}

メタデータのコレクションをファイルに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| メタデータ | IEnumerable`1 | メタデータのコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, Stream) {#exportasxml_2}

ドキュメント情報をストリームに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 文書情報です。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, string) {#exportasxml_3}

ドキュメント情報をファイルに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 文書情報です。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasxml_10}

テキスト領域のコレクションをストリームに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | テキスト領域のコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasxml_11}

テキスト領域の collectiob をファイルに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | テキスト領域のコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasxml_8}

テーブルのコレクションをストリームに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| tables | IEnumerable`1 | テーブルのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasxml_9}

テーブルのコレクションをファイルに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| tables | IEnumerable`1 | テーブルのコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasxml_6}

バーコードのコレクションをストリームに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| barcodes | IEnumerable`1 | バーコードのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasxml_7}

バーコードのコレクションをファイルに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| barcodes | IEnumerable`1 | バーコードのコレクションです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, Stream) {#exportasxml}

ドキュメントデータをストリームに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this DocumentData documentData, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentData | DocumentData | 文書データです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, string) {#exportasxml_1}

ドキュメントデータをファイルに XML 形式でエクスポートします。

```csharp
public static void ExportAsXml(this DocumentData documentData, string fileName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentData | DocumentData | 文書データです。 |
| fileName | 文字列 | 出力ファイルへの完全なパスです。 |

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
