---
title: "TemplateTable"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テンプレートテーブルを提供します。"
type: docs
weight: 160
url: /ja/net/groupdocs.parser.templates/templatetable/
---

## TemplateTable class

テンプレートテーブルを提供します。

```csharp
public sealed class TemplateTable : TemplateItem
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string) | [`TemplateTable`](../templatetable) クラスの新しいインスタンスを大文字の名前で初期化します。 |
| [TemplateTable](templatetable#constructor_3)(TemplateTableParameters, string) | [`TemplateTable`](../templatetable) クラスの新しいインスタンスを初期化します。 |
| [TemplateTable](templatetable#constructor_1)(TemplateTableLayout, string, double?) | [`TemplateTable`](../templatetable) クラスの新しいインスタンスを大文字の名前で初期化します。 |
| [TemplateTable](templatetable#constructor_4)(TemplateTableParameters, string, double?) | [`TemplateTable`](../templatetable) クラスの新しいインスタンスを初期化します。 |
| [TemplateTable](templatetable#constructor_2)(TemplateTableLayout, string, double?, bool) | [`TemplateTable`](../templatetable) クラスの新しいインスタンスを初期化します。 |
| [TemplateTable](templatetable#constructor_5)(TemplateTableParameters, string, double?, bool) | [`TemplateTable`](../templatetable) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | テーブルのレイアウトを取得します。 |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | テンプレート項目の名前を取得します。 |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | テンプレート項目の作成に使用されたページの幅を取得します。 |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | 自動モードでテーブルを検出するためのパラメータを取得します。 |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | `Name` が大文字に変換されたかどうかを示すブール値を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatetable/scale)(double) | 指定された係数でこのテンプレート項目を拡大縮小します。 |

### 備考

テーブルを定義する方法は2つあります：

* Using [`TemplateTableLayout`](../templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [`TemplateTableParameters`](../templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](../templatetableparameters) class for more information.

### 関連項目

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
