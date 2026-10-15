---
title: "WorksheetInfo"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "WorksheetInfogroupdocs.parser.data/worksheetinfo クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---

## WorksheetInfo constructor

[`WorksheetInfo`](../../worksheetinfo) クラスの新しいインスタンスを初期化します。

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| index | Int32 | ワークシートのゼロベースインデックス。 |
| name | 文字列 | ワークシート名を表す文字列値です。 |
| range | WorksheetRange | [`WorksheetRange`](../../worksheetrange) クラスのインスタンスで、ワークシートのサイズを表します。 |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | ワークシートのインデックスは負の値にできません。 |
| ArgumentNullException | ワークシートのサイズは `null` にできません。 |

### 関連項目

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
