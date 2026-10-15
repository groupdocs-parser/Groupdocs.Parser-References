---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "OCR 機能を提供します。"
type: docs
weight: 430
url: /ja/net/groupdocs.parser.options/ocrconnectorbase/
---

## OcrConnectorBase class

OCR 機能を提供します。

```csharp
public abstract class OcrConnectorBase
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| virtual [IsTextAreasSupported](../../groupdocs.parser.options/ocrconnectorbase/istextareassupported) { get; } | テキスト領域抽出がサポートされているかどうかを示す値を取得します。 |
| virtual [IsTextSupported](../../groupdocs.parser.options/ocrconnectorbase/istextsupported) { get; } | テキスト抽出がサポートされているかどうかを示す値を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| virtual [RecognizeText](../../groupdocs.parser.options/ocrconnectorbase/recognizetext#recognizetext)(Stream, OcrOptions) | *imageStream* ストリームからテキストを認識します。 |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas)(Stream, Page, OcrOptions) | *imageStream* ストリームからテキスト領域を認識します。 |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas_3)(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) | *imageStream* ストリームからテキスト領域を認識します。 |

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
