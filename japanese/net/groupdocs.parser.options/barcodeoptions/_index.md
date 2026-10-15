---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "バーコード抽出に使用されるオプションを提供します。"
type: docs
weight: 200
url: /ja/net/groupdocs.parser.options/barcodeoptions/
---

## BarcodeOptions class

バーコード抽出に使用されるオプションを提供します。

```csharp
public sealed class BarcodeOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [BarcodeOptions](barcodeoptions#constructor)() | [`BarcodeOptions`](../barcodeoptions) クラスの新しいインスタンスをデフォルト値で初期化します。 |
| [BarcodeOptions](barcodeoptions#constructor_1)(Rectangle) | [`BarcodeOptions`](../barcodeoptions) クラスの新しいインスタンスを矩形領域で初期化します。 |
| [BarcodeOptions](barcodeoptions#constructor_3)(QualityMode, QualityMode, params string[]) | [`BarcodeOptions`](../barcodeoptions) クラスの新しいインスタンスを品質設定とコードタイプで初期化します。 |
| [BarcodeOptions](barcodeoptions#constructor_2)(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) | [`BarcodeOptions`](../barcodeoptions) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AllowIncorrectBarcodes](../../groupdocs.parser.options/barcodeoptions/allowincorrectbarcodes) { get; set; } | 不正なバーコードが許可されているかどうかを示す値を取得します。 |
| [BarcodeQuality](../../groupdocs.parser.options/barcodeoptions/barcodequality) { get; set; } | ソースバーコードの品質を取得します。 |
| [CodeTypes](../../groupdocs.parser.options/barcodeoptions/codetypes) { get; set; } | 読み取るバーコードのタイプを取得します。 |
| [Dimension](../../groupdocs.parser.options/barcodeoptions/dimension) { get; set; } | バーコードの最小要素の最小サイズを取得します。 |
| [ImageQuality](../../groupdocs.parser.options/barcodeoptions/imagequality) { get; set; } | ソース画像の品質を取得します。 |
| [PagePreviewOptions](../../groupdocs.parser.options/barcodeoptions/pagepreviewoptions) { get; set; } | ドキュメントページのプレビューオプションを取得または設定します。 |
| [Rectangle](../../groupdocs.parser.options/barcodeoptions/rectangle) { get; set; } | ページ領域を含む矩形領域を取得します。 |

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
