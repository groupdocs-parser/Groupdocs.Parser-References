---
title: "PageTableArea"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テンプレートによる解析機能でテーブルを表すために使用されるテーブルページ領域を表します。"
type: docs
weight: 840
url: /ja/net/groupdocs.parser.data/pagetablearea/
---

## PageTableArea class

テンプレートによる解析機能でテーブルを表すために使用されるテーブルページ領域を表します。

```csharp
public sealed class PageTableArea : PageArea
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Cells](../../groupdocs.parser.data/pagetablearea/cells) { get; } | セルのコレクションを取得します。 |
| [ColumnCount](../../groupdocs.parser.data/pagetablearea/columncount) { get; } | テーブル列の総数を取得します。 |
| [Item](../../groupdocs.parser.data/pagetablearea/item) { get; } | 行と列のインデックスでテーブルセルを取得します。 |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | ページインデックスやページサイズなど、ドキュメントページ情報を取得します。 |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | 矩形領域を取得します。 |
| [RowCount](../../groupdocs.parser.data/pagetablearea/rowcount) { get; } | テーブル行の総数を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetColumnWidth](../../groupdocs.parser.data/pagetablearea/getcolumnwidth)(int) | 列幅を返します。 |
| [GetRowHeight](../../groupdocs.parser.data/pagetablearea/getrowheight)(int) | 行の高さを返します。 |

### 備考

[`PageTableArea`](../pagetablearea) class is used to organize inheritors of [`PageArea`](../pagearea) class in table structure.

### 関連項目

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
