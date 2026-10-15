---
title: "項目"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "行と列のインデックスでテーブルセルを取得します。"
type: docs
weight: 30
url: /ja/net/groupdocs.parser.data/pagetablearea/item/
---

## PageTableArea indexer

行と列のインデックスでテーブルセルを取得します。

```csharp
public PageTableAreaCell this[int rowIndex, int columnIndex] { get; }
```

| Parameter | 説明 |
| --- | --- |
| rowIndex | セル行のゼロベースインデックス。 |
| columnIndex | セル列のゼロベースインデックス。 |

### 戻り値

[`PageTableAreaCell`](../../pagetableareacell) クラスのインスタンスです。セルが見つからない場合は `null` です。

### 関連項目

* class [PageTableAreaCell](../../pagetableareacell)
* class [PageTableArea](../../pagetablearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
