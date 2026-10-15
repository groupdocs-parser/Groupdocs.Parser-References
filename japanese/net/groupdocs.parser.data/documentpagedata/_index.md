---
title: "DocumentPageData"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントページのデータを表します。ドキュメントページからのフィールドデータを含む FieldData./fielddata オブジェクトで構成されています。"
type: docs
weight: 740
url: /ja/net/groupdocs.parser.data/documentpagedata/
---

## DocumentPageData class

ドキュメントページのデータを表します。ドキュメントページからのフィールドデータを含む [`FieldData`](../fielddata) オブジェクトで構成されています。

```csharp
public sealed class DocumentPageData : DocumentData
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | フィールドデータの総数を取得します。 |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | インデックスでフィールドデータを取得します。 |
| [PageIndex](../../groupdocs.parser.data/documentpagedata/pageindex) { get; } | ページインデックスを取得します。 |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | テンプレートを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | フィールドデータの列挙子を返します。 |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | 名前が *fieldName* と等しいフィールドデータのコレクションを返します。 |

### 関連項目

* class [DocumentData](../documentdata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
