---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "OCR イベント用ハンドラを提供します。"
type: docs
weight: 440
url: /ja/net/groupdocs.parser.options/ocreventhandler/
---

## OcrEventHandler class

OCR イベント用ハンドラを提供します。

```csharp
public class OcrEventHandler
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [OcrEventHandler](ocreventhandler)() | [`OcrEventHandler`](../ocreventhandler)クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [HasWarnings](../../groupdocs.parser.options/ocreventhandler/haswarnings) { get; } | 警告リストが空でないかどうかを示す値を取得します。 |
| [Warnings](../../groupdocs.parser.options/ocreventhandler/warnings) { get; } | 警告メッセージのリストを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetWarnings](../../groupdocs.parser.options/ocreventhandler/getwarnings)(int) | ページ *pageIndex* の警告メッセージのリストを返します。 |
| virtual [OnWarnings](../../groupdocs.parser.options/ocreventhandler/onwarnings)(int, IList&lt;string&gt;) | ページの警告メッセージを設定します。 |

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
