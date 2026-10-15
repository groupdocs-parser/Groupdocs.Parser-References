---
title: "エクスポート"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "メタデータのコレクションをストリームにエクスポートします。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser.export/xmlexporter/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

メタデータのコレクションをストリームにエクスポートします。

```csharp
public override void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| メタデータ | IEnumerable`1 | メタデータのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

ドキュメント情報をストリームにエクスポートします。

```csharp
public override void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentInfo | IDocumentInfo | 文書情報です。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

テキスト領域のコレクションをストリームにエクスポートします。

```csharp
public override void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| textAreas | IEnumerable`1 | テキスト領域のコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

テーブルのコレクションをストリームにエクスポートします。

```csharp
public override void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| tables | IEnumerable`1 | テーブルのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

バーコードのコレクションをストリームにエクスポートします。

```csharp
public override void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| barcodes | IEnumerable`1 | バーコードのコレクションです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

ドキュメントデータをストリームにエクスポートします。

```csharp
public override void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| documentData | DocumentData | 文書データです。 |
| ストリーム | Stream | 出力ストリームです。 |

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
