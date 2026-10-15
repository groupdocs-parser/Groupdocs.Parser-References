---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ページ領域抽出に使用されるオプションを提供します。"
type: docs
weight: 460
url: /ja/net/groupdocs.parser.options/pageareaoptions/
---

## PageAreaOptions class

ページ領域抽出に使用されるオプションを提供します。

```csharp
public class PageAreaOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageAreaOptions](pageareaoptions#constructor)() | [`PageAreaOptions`](../pageareaoptions) クラスの新しいインスタンスを初期化します。 |
| [PageAreaOptions](pageareaoptions#constructor_1)(Rectangle) | [`PageAreaOptions`](../pageareaoptions) クラスの新しいインスタンスを初期化します。 |
| [PageAreaOptions](pageareaoptions#constructor_2)(Rectangle, double) | 無視される境界のサイズで [`PageAreaOptions`](../pageareaoptions) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | ページ領域を含む矩形領域を取得します。 |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | 矩形領域でキャプチャされる際に無視される境界のサイズを取得します。テキスト項目の高さの割合で測定されます。 |

### 備考

以下のメソッドでは、[`PageAreaOptions`](../pageareaoptions) クラスのインスタンスがパラメータとして使用されます：

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)

そこにある使用例をご覧ください。

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
