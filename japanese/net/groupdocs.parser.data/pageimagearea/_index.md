---
title: "ページ画像領域"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テンプレートによる解析機能でページ上の画像を表すために使用されるページ画像領域、またはメールや Zip アーカイブから抽出された画像が添付ファイルとしてある場合に使用されます。"
type: docs
weight: 830
url: /ja/net/groupdocs.parser.data/pageimagearea/
---

## PageImageArea class

テンプレートによる解析機能でページ上の画像を表すために使用されるページ画像領域、またはメールや Zip アーカイブから抽出された画像が添付ファイルとしてある場合に使用されます。

```csharp
public sealed class PageImageArea : PageArea
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | [`PageImageArea`](../pageimagearea) クラスの新しいインスタンスを初期化します。 |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | [`PageImageArea`](../pageimagearea) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | 画像の形式を取得します。 |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | ページインデックスやページサイズなど、ドキュメントページ情報を取得します。 |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | 矩形領域を取得します。 |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | 画像の回転角度を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | 画像ストリームを返します。 |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | 別の形式で画像ストリームを返します。 |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | 画像をファイルに保存します。 |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | 画像を別の形式でファイルに保存します。 |

### 備考

以下のメソッドの戻り値として、[`PageImageArea`](../pageimagearea) クラスのインスタンスが使用されます。

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

そこにある使用例をご覧ください。

### 関連項目

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
