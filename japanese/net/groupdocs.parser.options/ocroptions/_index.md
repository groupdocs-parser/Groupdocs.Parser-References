---
title: "OcrOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "OCR コネクタに使用されるオプションを提供します。"
type: docs
weight: 450
url: /ja/net/groupdocs.parser.options/ocroptions/
---

## OcrOptions class

OCR コネクタに使用されるオプションを提供します。

```csharp
public class OcrOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [OcrOptions](ocroptions#constructor)() | 矩形領域を使用して、[`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |
| [OcrOptions](ocroptions#constructor_5)(OcrEventHandler) | [`OcrEventHandler`](../ocreventhandler) オブジェクトを使用して、[`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |
| [OcrOptions](ocroptions#constructor_6)(PagePreviewOptions) | 矩形領域を使用して、[`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |
| [OcrOptions](ocroptions#constructor_1)(Rectangle) | 矩形領域を使用して、[`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |
| [OcrOptions](ocroptions#constructor_2)(Rectangle, OcrEventHandler) | 矩形領域と[`OcrEventHandler`](../ocreventhandler) オブジェクトを使用して、[`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |
| [OcrOptions](ocroptions#constructor_3)(Rectangle, OcrEventHandler, PagePreviewOptions, bool) | [`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |
| [OcrOptions](ocroptions#constructor_4)(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) | [`OcrOptions`](../ocroptions) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Handler](../../groupdocs.parser.options/ocroptions/handler) { get; set; } | OCR イベントを捕捉するためのイベントハンドラを取得します。 |
| [Language](../../groupdocs.parser.options/ocroptions/language) { get; set; } | OCR に使用される言語を取得または設定します。認識時に使用されるアルファベットを決定します。デフォルトでは英語が使用されます。 |
| [PagePreviewOptions](../../groupdocs.parser.options/ocroptions/pagepreviewoptions) { get; set; } | ドキュメントページのプレビューオプションを取得します。 |
| [Rectangle](../../groupdocs.parser.options/ocroptions/rectangle) { get; set; } | テキスト認識に使用されるページ領域を制限する矩形領域を取得します。 |
| [UseSpellChecker](../../groupdocs.parser.options/ocroptions/usespellchecker) { get; set; } | スペルチェッカーが使用されているかどうかを示す値を取得します。 |

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
