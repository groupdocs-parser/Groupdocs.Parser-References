---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ページがどのようにレンダリングされるかの情報を表します。"
type: docs
weight: 500
url: /ja/net/groupdocs.parser.options/pagerenderinfo/
---

## PageRenderInfo class

ページがどのようにレンダリングされるかの情報を表します。

```csharp
public sealed class PageRenderInfo
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageRenderInfo](pagerenderinfo)(int, int, int) | 新しいインスタンスを初期化します [`PageRenderInfo`](../pagerenderinfo) クラス。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [ColumnCount](../../groupdocs.parser.options/pagerenderinfo/columncount) { get; } | タイル列の総数を取得します。 |
| [PageNumber](../../groupdocs.parser.options/pagerenderinfo/pagenumber) { get; } | ページ番号を取得します。 |
| [RowCount](../../groupdocs.parser.options/pagerenderinfo/rowcount) { get; } | タイル行の総数を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetColumn](../../groupdocs.parser.options/pagerenderinfo/getcolumn)(int) | タイル *tileIndex* が配置されている列のインデックスを返します。 |
| [GetRow](../../groupdocs.parser.options/pagerenderinfo/getrow)(int) | タイル *tileIndex* が配置されている行のインデックスを返します。 |

### 備考

一部のドキュメント（例としてスプレッドシート）は、ページを単一の画像としてレンダリングできません。そのようなドキュメントでは、ページがタイルの集合としてレンダリングされます。これらのタイルは長方形のテーブルに配置されます。

[`RowCount`](./rowcount) and [`ColumnCount`](./columncount) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
