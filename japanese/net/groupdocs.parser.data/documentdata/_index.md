---
title: "DocumentData"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "文書のデータを表します。FieldData./fielddata オブジェクトで構成されており、文書からのフィールドデータを含みます。"
type: docs
weight: 730
url: /ja/net/groupdocs.parser.data/documentdata/
---

## DocumentData class

文書のデータを表します。[`FieldData`](../fielddata) オブジェクトで構成されており、文書からのフィールドデータを含みます。

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | フィールドデータの総数を取得します。 |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | インデックスでフィールドデータを取得します。 |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | テンプレートを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | フィールドデータの列挙子を返します。 |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | 名前が *fieldName* と等しいフィールドデータのコレクションを返します。 |

### 備考

[`DocumentData`](../documentdata) クラスのインスタンスは、[`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) および [`ParseForm`](../../groupdocs.parser/parser/parseform) メソッドの戻り値として使用されます。使用例をご覧ください。

### 関連項目

* class [FieldData](../fielddata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
