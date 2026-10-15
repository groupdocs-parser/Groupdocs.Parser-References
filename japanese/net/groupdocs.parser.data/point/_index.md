---
title: "Point"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "点を表します。"
type: docs
weight: 870
url: /ja/net/groupdocs.parser.data/point/
---

## Point class

点を表します。

```csharp
public sealed class Point : IEquatable<Point>
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [Point](point)(double, double) | [`Point`](../point) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [X](../../groupdocs.parser.data/point/x) { get; } | X 座標を取得します。 |
| [Y](../../groupdocs.parser.data/point/y) { get; } | Y 座標を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [Parse](../../groupdocs.parser.data/point/parse)(string) | ポイントの文字列表現をクラスの等価オブジェクトに変換します。 |
| override [Equals](../../groupdocs.parser.data/point/equals#equals_1)(object) | 現在の [`Point`](../point) が指定されたオブジェクトと同じかどうかを判断します。 |
| [Equals](../../groupdocs.parser.data/point/equals#equals)(Point) | 現在の [`Point`](../point) が指定された [`Point`](../point) オブジェクトと同じかどうかを判断します。 |
| override [GetHashCode](../../groupdocs.parser.data/point/gethashcode)() | 現在の [`Point`](../point) オブジェクトのハッシュコードを返します。 |
| override [ToString](../../groupdocs.parser.data/point/tostring)() | このインスタンスの値を文字列に変換します。 |
| static [TryParse](../../groupdocs.parser.data/point/tryparse)(string, out Point) | ポイントの文字列表現をクラスの等価オブジェクトに変換します。戻り値は変換が成功したか失敗したかを示します。 |
| [operator ==](../../groupdocs.parser.data/point/op_equality) | 2 つの [`Point`](../point) オブジェクトが同じかどうかを判断します。 |
| [operator !=](../../groupdocs.parser.data/point/op_inequality) | 2 つの [`Point`](../point) オブジェクトが異なるかどうかを判断します。 |

### 関連項目

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
