---
title: TemplateFixedPosition
second_title: GroupDocs.Parser for .NET API リファレンス
description: 長方形領域によって定義されるテンプレート フィールド位置を提供します
type: docs
weight: 680
url: /ja/net/groupdocs.parser.templates/templatefixedposition/
---
## TemplateFixedPosition class

長方形領域によって定義されるテンプレート フィールド位置を提供します。

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | の新しいインスタンスを初期化します[`TemplateFixedPosition`](../templatefixedposition)class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | テンプレート フィールドを含む四角形の領域を取得します。 |

### 例

これは、フィールドの位置を定義する最も簡単な方法です。 フィールド値の境界となる長方形の領域をページに設定する必要があります。 長方形の領域に含まれるすべてのテキスト (部分的であっても) が値として抽出されます。

```csharp
// 位置 (35, 160) でサイズ (110, 20) の長方形で囲まれた "Address" という名前の固定テンプレート フィールドを作成します。
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### 関連項目

* class [TemplatePosition](../templateposition)
* 名前空間 [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* 組み立て [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
