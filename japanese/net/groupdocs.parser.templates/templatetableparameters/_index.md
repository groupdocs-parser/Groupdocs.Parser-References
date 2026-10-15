---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テーブル検出アルゴリズム用のパラメータを提供します。"
type: docs
weight: 180
url: /ja/net/groupdocs.parser.templates/templatetableparameters/
---

## TemplateTableParameters class

テーブル検出アルゴリズム用のパラメータを提供します。

```csharp
public sealed class TemplateTableParameters
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | [`TemplateTableParameters`](../templatetableparameters) クラスの新しいインスタンスを初期化します。 |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | [`TemplateTableParameters`](../templatetableparameters) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | テーブルに結合されたセルがあるかどうかを示す値を取得します。 |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | テーブル列の最小数を取得します。 |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | テーブル行の最小数を取得します。 |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | テーブル列間の最小スペースを取得します。 |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | テーブルを含む矩形領域を取得します。 |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | テーブル列の区切り文字を取得します。 |

### 備考

テーブルを検出するためのアルゴリズムは2つあります：

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

アルゴリズムがテーブルを検出できない、または正確に検出できない場合、[`TemplateTableLayout`](../templatetablelayout) クラスが使用されます。

### 関連項目

* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
