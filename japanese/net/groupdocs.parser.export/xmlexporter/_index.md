---
title: "XmlExporter"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "XML 形式でデータをエクスポートする機能を提供します。"
type: docs
weight: 660
url: /ja/net/groupdocs.parser.export/xmlexporter/
---

## XmlExporter class

XML 形式でデータをエクスポートする機能を提供します。

```csharp
public sealed class XmlExporter : ExporterBase
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [XmlExporter](xmlexporter)() | デフォルトコンストラクタです。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export)(DocumentData, Stream) | ドキュメントデータをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export)(DocumentData, string) | ドキュメントデータをファイルにエクスポートします。 |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_2)(IDocumentInfo, Stream) | ドキュメント情報をストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IDocumentInfo, string) | ドキュメント情報をファイルにエクスポートします。 |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | メタデータのコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;MetadataItem&gt;, string) | メタデータのコレクションをファイルにエクスポートします。 |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | バーコードのコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageBarcodeArea&gt;, string) | バーコードのコレクションをファイルにエクスポートします。 |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | テーブルのコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTableArea&gt;, string) | テーブルのコレクションをファイルにエクスポートします。 |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | テキスト領域のコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTextArea&gt;, string) | テキスト領域のコレクションをファイルにエクスポートします。 |

### 関連項目

* class [ExporterBase](../exporterbase)
* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
