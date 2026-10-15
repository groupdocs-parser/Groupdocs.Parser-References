---
title: "RecognizeText"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "imageStream ストリームからテキストを認識します。"
type: docs
weight: 30
url: /ja/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---

## OcrConnectorBase.RecognizeText method

*imageStream* ストリームからテキストを認識します。

```csharp
public virtual string RecognizeText(Stream imageStream, OcrOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| imageStream | Stream | ドキュメントページの画像表現です。 |
| options | OcrOptions | OCR オプションです。 |

### 戻り値

認識されたテキストを表す文字列です。テキスト認識がサポートされていない場合は `null` です。

### 関連項目

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
