---
title: "HighlightOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "検索シナリオで見つかったテキストの周囲のテキストブロックをハイライト抽出するために使用されるオプションを提供します。"
type: docs
weight: 360
url: /ja/net/groupdocs.parser.options/highlightoptions/
---

## HighlightOptions class

ハイライト（検索シナリオで見つかったテキストの周囲のテキストブロック）を抽出するために使用されるオプションを提供します。

```csharp
public sealed class HighlightOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)() | 固定長ハイライトを抽出するために使用される [`HighlightOptions`](../highlightoptions) クラスの新しいインスタンスを初期化します。 |
| [HighlightOptions](highlightoptions#constructor_1)(int) | 固定長ハイライトを抽出するために使用される [`HighlightOptions`](../highlightoptions) クラスの新しいインスタンスを初期化します。 |
| [HighlightOptions](highlightoptions#constructor_2)(int?, bool) | 行制限ハイライトを抽出するために使用される [`HighlightOptions`](../highlightoptions) クラスの新しいインスタンスを初期化します。 |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int) | 固定語数ハイライトを抽出するために使用される [`HighlightOptions`](../highlightoptions) クラスの新しいインスタンスを初期化します。 |
| [HighlightOptions](highlightoptions#constructor_4)(int?, int?, bool) | 新しいインスタンスを初期化します [`HighlightOptions`](../highlightoptions) クラス。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; set; } | ハイライト抽出がテキスト行の開始（または終了）で制限されるかどうかを示す値を取得します。 |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; set; } | 最大テキスト長を取得します。 |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; set; } | 最大語数を取得します。 |

### 備考

インスタンス [`HighlightOptions`](../highlightoptions) クラスは、[`GetHighlight`](../../groupdocs.parser/parser/gethighlight) メソッドのパラメータとして使用されます。使用例はそちらをご覧ください。

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
