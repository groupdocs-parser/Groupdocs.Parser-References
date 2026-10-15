---
title: "TextOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テキスト抽出に使用されるオプションを提供します。"
type: docs
weight: 610
url: /ja/net/groupdocs.parser.options/textoptions/
---

## TextOptions class

テキスト抽出に使用されるオプションを提供します。

```csharp
public sealed class TextOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [TextOptions](textoptions#constructor)() | [`TextOptions`](../textoptions) クラスの新しいインスタンスを初期化します。 |
| [TextOptions](textoptions#constructor_1)(bool) | [`TextOptions`](../textoptions) クラスの新しいインスタンスを初期化します。 |
| [TextOptions](textoptions#constructor_2)(bool, bool) | OCR 使用オプションとともに、[`TextOptions`](../textoptions) クラスの新しいインスタンスを初期化します。 |
| [TextOptions](textoptions#constructor_3)(bool, bool, OcrOptions) | [`TextOptions`](../textoptions) クラスの新しいインスタンスを初期化します。OCR オプションを設定できるように。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IncludeAnnotations](../../groupdocs.parser.options/textoptions/includeannotations) { get; set; } | 注釈が含まれるかどうかを示す値を取得します。デフォルト値は `false` です。 |
| [OcrOptions](../../groupdocs.parser.options/textoptions/ocroptions) { get; set; } | OCR 機能の追加オプションを取得します。 |
| [UseOcr](../../groupdocs.parser.options/textoptions/useocr) { get; set; } | OCR コネクタがテキスト抽出に使用されているかどうかを示す値を取得します。 |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; set; } | 生モードが使用されているかどうかを示す値を取得します。 |

### 備考

[`TextOptions`](../textoptions) クラスのインスタンスは、[`GetText`](../../groupdocs.parser/parser/gettext) と [`GetText`](../../groupdocs.parser/parser/gettext) メソッドのパラメータとして使用されます。使用例をご確認ください。

テキスト抽出の生モードを指定するために使用されます。このモードでは、テキストは正確さは低いものの標準モードよりも高速に抽出されます。生モードがドキュメント形式をサポートしない場合、このパラメータは無視され、標準モードが使用されます。

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
