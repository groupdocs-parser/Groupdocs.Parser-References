---
title: "テンプレート"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "文書ページテンプレートを提供します。TemplateItem./templateitem オブジェクトで構成され、テキストフィールドやテーブル定義などテンプレートの項目を表します。"
type: docs
weight: 50
url: /ja/net/groupdocs.parser.templates/template/
---

## Template class

文書ページテンプレートを提供します。[`TemplateItem`](../templateitem) オブジェクトで構成され、テキストフィールドやテーブル定義などテンプレートの項目を表します。

```csharp
public sealed class Template : IEnumerable<TemplateItem>
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [Template](template#constructor)(IEnumerable&lt;TemplateItem&gt;) | [`Template`](../template) クラスの新しいインスタンスを初期化します。 |
| [Template](template#constructor_1)(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) | テンプレートオプションを指定して、[`Template`](../template) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Count](../../groupdocs.parser.templates/template/count) { get; } | テンプレート項目の総数を取得します。 |
| [IsOcrCompatible](../../groupdocs.parser.templates/template/isocrcompatible) { get; } | テンプレートが OCR と互換性があるかどうかを示す値を取得します。 |
| [Item](../../groupdocs.parser.templates/template/item) { get; } | インデックスでテンプレート項目を取得します。 |
| [Options](../../groupdocs.parser.templates/template/options) { get; } | テンプレートオプションを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [Load](../../groupdocs.parser.templates/template/load#load)(Stream) | ストリームからテンプレートを読み込みます。 |
| static [Load](../../groupdocs.parser.templates/template/load#load_1)(string) | ファイルからテンプレートを読み込みます。 |
| [GetEnumerator](../../groupdocs.parser.templates/template/getenumerator)() | テンプレート項目の列挙子を返します。 |
| [Save](../../groupdocs.parser.templates/template/save#save)(Stream) | テンプレートをストリームに保存します。 |
| [Save](../../groupdocs.parser.templates/template/save#save_1)(string) | テンプレートをファイルに保存します。 |

### 備考

**Learn more:**

* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)

### 関連項目

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
