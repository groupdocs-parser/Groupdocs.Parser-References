---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ページテキスト領域の抽出に使用されるオプションを提供します。"
type: docs
weight: 520
url: /ja/net/groupdocs.parser.options/pagetextareaoptions/
---

## PageTextAreaOptions class

ページテキスト領域の抽出に使用されるオプションを提供します。

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)() | OCR使用オプションを指定して、[`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool) | OCR使用オプションを指定して、[`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string) | 正規表現を使用して、[`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。他のオプションはデフォルトで設定されます（詳細は備考をご参照ください）。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(bool, OcrOptions) | OCRオプションを設定できるように、[`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_6)(string, Rectangle) | 正規表現と矩形領域を使用して、[`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。他のオプションはデフォルトで設定されます（詳細は備考をご参照ください）。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_7)(string, Rectangle, double) | 正規表現、矩形領域、および無視する境界のサイズを指定して、[`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。他のオプションはデフォルトで設定されます（詳細は備考をご参照ください）。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, bool, bool, bool, Rectangle) | [`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
| [PageTextAreaOptions](pagetextareaoptions#constructor_5)(string, bool, bool, bool, Rectangle, double) | [`PageTextAreaOptions`](../pagetextareaoptions) クラスの新しいインスタンスを、無視される境界のサイズで初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; set; } | 正規表現を取得します。 |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; set; } | テキスト書式が無視されているかどうかを示す値を取得します。 |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; set; } | テキストの大文字小文字が無視されていないかどうかを示す値を取得します。 |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; set; } | OCR 機能の追加オプションを取得します。 |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | ページ領域を含む矩形領域を取得します。 |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | 矩形領域でキャプチャされる際に無視される境界のサイズを取得します。テキスト項目の高さの割合で測定されます。 |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; set; } | セグメントが結合されているかどうかを示す値を取得します。 |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; set; } | テキスト領域の抽出に OCR 機能が使用されているかどうかを示す値を取得します。 |

### 備考

[`PageTextAreaOptions`](../pagetextareaoptions) クラスのインスタンスは、[`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) および [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) メソッドのパラメーターとして使用されます。使用例をご覧ください。 **詳細を見る:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 関連項目

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
