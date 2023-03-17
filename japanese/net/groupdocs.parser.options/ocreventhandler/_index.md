---
title: OcrEventHandler
second_title: GroupDocs.Parser for .NET API リファレンス
description: OCR イベントのハンドラーを提供します
type: docs
weight: 490
url: /ja/net/groupdocs.parser.options/ocreventhandler/
---
## OcrEventHandler class

OCR イベントのハンドラーを提供します。

```csharp
public class OcrEventHandler
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [OcrEventHandler](ocreventhandler)() | の新しいインスタンスを初期化します[`OcrEventHandler`](../ocreventhandler)class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [HasWarnings](../../groupdocs.parser.options/ocreventhandler/haswarnings) { get; } | 警告のリストが空でないかどうかを示す値を取得します。 |
| [Warnings](../../groupdocs.parser.options/ocreventhandler/warnings) { get; } | 警告メッセージのリストを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetWarnings](../../groupdocs.parser.options/ocreventhandler/getwarnings)(int) | を含むページの警告メッセージのリストを返します*pageIndex*. |
| virtual [OnWarnings](../../groupdocs.parser.options/ocreventhandler/onwarnings)(int, IList&lt;string&gt;) | ページの警告メッセージを設定します。 |

### 関連項目

* 名前空間 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 組み立て [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->