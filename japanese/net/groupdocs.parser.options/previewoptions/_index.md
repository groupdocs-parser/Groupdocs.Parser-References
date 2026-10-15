---
title: "PreviewOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。"
type: docs
weight: 550
url: /ja/net/groupdocs.parser.options/previewoptions/
---

## PreviewOptions class

プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。

```csharp
public class PreviewOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | 出力ストリームが閉じられるように、[`PreviewOptions`](../previewoptions) クラスの新しいインスタンスを初期化します。 |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | 出力ストリームがクライアントに返され、さらに使用できるように、[`PreviewOptions`](../previewoptions) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CreatePageStream](../../groupdocs.parser.options/previewoptions/createpagestream) { get; set; } | ページストリーム作成デリゲートのインスタンスを取得または設定します。 |
| [Dpi](../../groupdocs.parser.options/previewoptions/dpi) { get; set; } | dpi を取得または設定します。 |
| [Height](../../groupdocs.parser.options/previewoptions/height) { get; set; } | ページプレビューの高さを取得または設定します。 |
| [PageNumbers](../../groupdocs.parser.options/previewoptions/pagenumbers) { get; set; } | プレビューを生成するページ番号の配列を取得または設定します。 |
| [PreviewFormat](../../groupdocs.parser.options/previewoptions/previewformat) { get; set; } | プレビュー画像の形式を取得または設定します。 |
| [PreviewPageRender](../../groupdocs.parser.options/previewoptions/previewpagerender) { get; set; } | ページプレビュー描画情報デリゲートのインスタンスを取得または設定します。 |
| [ReleasePageStream](../../groupdocs.parser.options/previewoptions/releasepagestream) { get; set; } | ページプレビュー完了デリゲートのインスタンスを取得または設定します。 |
| [Width](../../groupdocs.parser.options/previewoptions/width) { get; set; } | ページプレビューの幅を取得または設定します。 |

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
