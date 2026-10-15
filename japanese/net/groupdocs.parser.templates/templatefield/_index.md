---
title: "TemplateField"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テンプレートのテキストフィールドを提供します。"
type: docs
weight: 80
url: /ja/net/groupdocs.parser.templates/templatefield/
---

## TemplateField class

テンプレートのテキストフィールドを提供します。

```csharp
public sealed class TemplateField : TemplateItem
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | `[`TemplateField`](../templatefield)` クラスの新しいインスタンスを初期化します。 |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, double?) | `[`TemplateField`](../templatefield)` クラスの新しいインスタンスを初期化します。 |
| [TemplateField](templatefield#constructor_2)(TemplatePosition, string, double?, bool) | `[`TemplateField`](../templatefield)` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IsHidden](../../groupdocs.parser.templates/templatefield/ishidden) { get; set; } | 非表示テンプレートフィールドフラグを取得または設定します。 |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | テンプレート項目の名前を取得します。 |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | テンプレート項目の作成に使用されたページの幅を取得します。 |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | ドキュメントページ上でテンプレートフィールドを見つける方法を記述する値を取得します。 |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | `Name` が大文字に変換されたかどうかを示すブール値を取得します。 |
| [Value](../../groupdocs.parser.templates/templatefield/value) { get; set; } | テンプレートフィールドの値を取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatefield/scale)(double) | 指定された係数でこのテンプレート項目を拡大縮小します。 |

### 備考

テキストフィールドはページ上の位置で定義されます。テキストフィールドを定義する方法は3つあります：

* [`Using the rectangular area`](../templatefixedposition)
* [`Using the regular expression`](../templateregexposition)
* [`Using the linked field`](../templatelinkedposition)

### 関連項目

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
