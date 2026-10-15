---
title: "ExporterBase"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "データエクスポート機能の基底クラスを提供します。"
type: docs
weight: 630
url: /ja/net/groupdocs.parser.export/exporterbase/
---

## ExporterBase class

データエクスポート機能の基底クラスを提供します。

```csharp
public abstract class ExporterBase
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export)(DocumentData, Stream) | ドキュメントデータをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_1)(DocumentData, string) | ドキュメントデータをファイルにエクスポートします。 |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_2)(IDocumentInfo, Stream) | ドキュメント情報をストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_3)(IDocumentInfo, string) | ドキュメント情報をファイルにエクスポートします。 |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | メタデータのコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_5)(IEnumerable&lt;MetadataItem&gt;, string) | メタデータのコレクションをファイルにエクスポートします。 |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | バーコードのコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_7)(IEnumerable&lt;PageBarcodeArea&gt;, string) | バーコードのコレクションをファイルにエクスポートします。 |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | テーブルのコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_9)(IEnumerable&lt;PageTableArea&gt;, string) | テーブルのコレクションをファイルにエクスポートします。 |
| abstract [Export](../../groupdocs.parser.export/exporterbase/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | テキスト領域のコレクションをストリームにエクスポートします。 |
| [Export](../../groupdocs.parser.export/exporterbase/export#export_11)(IEnumerable&lt;PageTextArea&gt;, string) | テキスト領域のコレクションをファイルにエクスポートします。 |

### 関連項目

* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
