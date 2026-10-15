---
title: "PageTextArea"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テンプレート解析またはフォーム解析機能でテキスト値を表すために使用されるページテキスト領域を表します。"
type: docs
weight: 860
url: /ja/net/groupdocs.parser.data/pagetextarea/
---

## PageTextArea class

テンプレート解析またはフォーム解析機能でテキスト値を表すために使用されるページテキスト領域を表します。

```csharp
public sealed class PageTextArea : PageArea
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | [`PageTextArea`](../pagetextarea) クラスの新しいインスタンスを初期化します。 |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | [`PageTextArea`](../pagetextarea) クラスの新しいインスタンスを初期化します。 |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | [`PageTextArea`](../pagetextarea) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | 子テキストページ領域のコレクションを取得します。 |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | ベースラインを取得します。 |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | ページインデックスやページサイズなど、ドキュメントページ情報を取得します。 |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | 矩形領域を取得します。 |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | テキストを取得します。 |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | フォントサイズやフォント名などのテキストスタイルを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | このインスタンスの値を文字列に変換します。 |

### 備考

以下のメソッドの戻り値として、[`PageTextArea`](../pagetextarea) クラスのインスタンスが使用されます。

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

また、[`PageTextArea`](../pagetextarea) クラスのインスタンスが、[`PageArea`](../fielddata/pagearea) プロパティの値として使用されます。

そこにある使用例をご覧ください。

テキスト領域は単一または複合のいずれかです。最初の場合、矩形領域で囲まれたテキストを含みます。2番目の場合、他のテキスト領域を含み、テキストおよびテーブルのプロパティは子テキスト領域によって計算されます。

### 関連項目

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
