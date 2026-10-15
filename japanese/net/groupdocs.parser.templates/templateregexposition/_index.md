---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "正規表現を使用するテンプレートフィールドの位置を提供します。"
type: docs
weight: 150
url: /ja/net/groupdocs.parser.templates/templateregexposition/
---

## TemplateRegexPosition class

正規表現を使用するテンプレートフィールドの位置を提供します。

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | `[`TemplateRegexPosition`](../templateregexposition)` クラスの新しいインスタンスを初期化します。 |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | `[`TemplateRegexPosition`](../templateregexposition)` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | 正規表現を取得します。 |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | テキストの大文字小文字が無視されていないかどうかを示す値を取得します。 |

### 例

次の例は、ドキュメントに \"Invoice Number INV-12345\" が含まれている場合の状況を示し、テンプレートフィールドを以下のように定義できることを示します：

```csharp
// 「InvoiceNumber」名前の正規表現テンプレートフィールドを作成します
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

この場合、値として文字列全体が抽出されます。文字列の一部だけを抽出するには、正規表現グループ \"value\" を使用します：

```csharp
// 「InvoiceNumber」名前で「value」グループを持つ正規表現テンプレートフィールドを作成します
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

この場合、値として \"INV-3337\" 文字列が抽出されます。

### 関連項目

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
