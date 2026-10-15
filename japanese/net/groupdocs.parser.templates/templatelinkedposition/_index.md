---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "リンクされたフィールドを使用するテンプレートフィールドの位置を提供します。"
type: docs
weight: 110
url: /ja/net/groupdocs.parser.templates/templatelinkedposition/
---

## TemplateLinkedPosition class

リンクされたフィールドを使用するテンプレートフィールドの位置を提供します。

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | 新しいインスタンスを初期化します [`TemplateLinkedPosition`](../templatelinkedposition) クラス。 |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | `[`TemplateLinkedPosition`](../templatelinkedposition)` クラスの新しいインスタンスを、UPPER CASE linked field name とともに初期化します。 |
| [TemplateLinkedPosition](templatelinkedposition#constructor_2)(string, Size, TemplateLinkedPositionEdges, bool, bool) | 新しいインスタンスを初期化します [`TemplateLinkedPosition`](../templatelinkedposition) クラス。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | `[`SearchArea`](./searcharea)` がリンクフィールドのサイズでスケーリングされているかどうかを示す値を取得します。 |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | フィールドが検索されるリンクフィールドのエッジを取得します。 |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | リンクフィールド名を取得します。 |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | フィールドが検索される領域のサイズを取得します。 |

### 例

以下の例は、請求書番号フィールドが "Invoice number" 文字列の右側に配置されていることが分かっている場合のコードを示しています。次のコードが使用されます：

```csharp
// 「Invoice Number」テキストを検索する正規表現テンプレートフィールドを作成します
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// 「Invoice」フィールドに関連付けられた関連テンプレートフィールドを作成し、その右側の値を抽出します
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### 関連項目

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
