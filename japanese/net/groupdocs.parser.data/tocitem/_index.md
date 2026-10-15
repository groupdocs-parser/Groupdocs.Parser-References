---
title: "TocItem"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "目次抽出機能で使用される項目を表します。"
type: docs
weight: 920
url: /ja/net/groupdocs.parser.data/tocitem/
---

## TocItem class

目次抽出機能で使用される項目を表します。

```csharp
public class TocItem
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TocItem](tocitem)(int, string, int?) | [`TocItem`](../tocitem) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Depth](../../groupdocs.parser.data/tocitem/depth) { get; } | 深さレベルを取得します。 |
| [PageIndex](../../groupdocs.parser.data/tocitem/pageindex) { get; } | ページインデックスを取得します。 |
| [Text](../../groupdocs.parser.data/tocitem/text) { get; } | テキストを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| virtual [ExtractText](../../groupdocs.parser.data/tocitem/extracttext)() | [`TocItem`](../tocitem) オブジェクトが参照するドキュメントからテキストを抽出します。 |

### 備考

[`TocItem`](../tocitem) クラスのインスタンスは、[`GetToc`](../../groupdocs.parser/parser/gettoc) メソッドの戻り値として使用されます。使用例をご参照ください。

### 関連項目

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
