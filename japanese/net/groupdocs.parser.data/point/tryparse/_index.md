---
title: "TryParse"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ポイントの文字列表現をクラスの等価オブジェクトに変換します。戻り値は変換が成功したか失敗したかを示します。"
type: docs
weight: 80
url: /ja/net/groupdocs.parser.data/point/tryparse/
---

## Point.TryParse method

ポイントの文字列表現をクラスの等価オブジェクトに変換します。戻り値は変換が成功したか失敗したかを示します。

```csharp
public static bool TryParse(string s, out Point point)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| s | 文字列 | 変換するポイントを含む文字列です。 |
| point | Point& | メソッドが戻ると、変換が成功した場合は *s* パラメーターで指定された値と等価な [`Point`](../../point) クラスのインスタンスが含まれます。失敗した場合は `null` です。 |

### 戻り値

*s* が正常に変換された場合は `true`、それ以外の場合は `false` です。

### 関連項目

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
