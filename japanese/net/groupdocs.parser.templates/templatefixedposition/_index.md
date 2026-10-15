---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "矩形領域で定義されたテンプレートフィールドの位置を提供します。"
type: docs
weight: 90
url: /ja/net/groupdocs.parser.templates/templatefixedposition/
---

## TemplateFixedPosition class

矩形領域で定義されたテンプレートフィールドの位置を提供します。

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | `[`TemplateFixedPosition`](../templatefixedposition)` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | テンプレートフィールドを含む矩形領域を取得します。 |

### 例

これはフィールド位置を定義する最も簡単な方法です。ページ上にフィールド値を囲む矩形領域を設定する必要があります。矩形領域内に含まれる（部分的であっても）すべてのテキストが値として抽出されます：

```csharp
// 位置 (35, 160) に矩形で囲まれ、サイズ (110, 20) の「Address」名の固定テンプレートフィールドを作成します
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### 関連項目

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
