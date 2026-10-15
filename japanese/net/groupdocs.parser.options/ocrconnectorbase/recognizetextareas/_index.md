---
title: "RecognizeTextAreas"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "imageStream ストリームからテキスト領域を認識します。"
type: docs
weight: 40
url: /ja/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---

## RecognizeTextAreas(Stream, Page, OcrOptions) {#recognizetextareas}

*imageStream* ストリームからテキスト領域を認識します。

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, Page page, 
    OcrOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| imageStream | Stream | ドキュメントページの画像表現です。 |
| page | Page | ドキュメントページです。 |
| options | OcrOptions | OCR オプションです。 |

### 戻り値

[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。テキスト領域の認識がサポートされていない場合は `null` です。

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## RecognizeTextAreas(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) {#recognizetextareas_3}

*imageStream* ストリームからテキスト領域を認識します。

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, 
    IEnumerable<Rectangle> rectangles, string allowedSymbols, Page page, OcrOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| imageStream | Stream | ドキュメントページの画像表現です。 |
| rectangles | IEnumerable`1 | OCR 機能を制限する矩形領域のコレクションです。 |
| allowedSymbols | 文字列 | OCR による許可シンボルのフィルタです。 |
| page | Page | ドキュメントページです。 |
| options | OcrOptions | OCR オプションです。 |

### 戻り値

[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。テキスト領域の認識がサポートされていない場合は `null` です。

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
