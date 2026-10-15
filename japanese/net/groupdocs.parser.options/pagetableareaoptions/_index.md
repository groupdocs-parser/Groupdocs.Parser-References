---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ページテーブル領域の抽出に使用されるオプションを提供します。"
type: docs
weight: 510
url: /ja/net/groupdocs.parser.options/pagetableareaoptions/
---

## PageTableAreaOptions class

ページテーブル領域の抽出に使用されるオプションを提供します。

```csharp
public sealed class PageTableAreaOptions : PageAreaOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageTableAreaOptions](pagetableareaoptions)(TemplateTableLayout) | [`PageAreaOptions`](../pageareaoptions) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | ページ領域を含む矩形領域を取得します。 |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | 矩形領域でキャプチャされる際に無視される境界のサイズを取得します。テキスト項目の高さの割合で測定されます。 |
| [TableLayout](../../groupdocs.parser.options/pagetableareaoptions/tablelayout) { get; } | ページ上のテーブルを定義するテーブルレイアウトを取得します。 |

### 備考

[`PageTableAreaOptions`](../pagetableareaoptions) クラスのインスタンスは、[`GetTables`](../../groupdocs.parser/parser/gettables) および [`GetTables`](../../groupdocs.parser/parser/gettables) メソッドのパラメーターとして使用されます。使用例はそちらをご覧ください。

### 関連項目

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
