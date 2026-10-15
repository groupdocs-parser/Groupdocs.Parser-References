---
title: "ParserSettings"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "データ抽出をカスタマイズするために使用される設定を提供します。"
type: docs
weight: 540
url: /ja/net/groupdocs.parser.options/parsersettings/
---

## ParserSettings class

データ抽出をカスタマイズするために使用される設定を提供します。

```csharp
public sealed class ParserSettings
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [ParserSettings](parsersettings#constructor)(ExternalResourceHandler) | [`ParserSettings`](../parsersettings) クラスの新しいインスタンスを外部リソースハンドラと共に初期化します。 |
| [ParserSettings](parsersettings#constructor_1)(ILogger) | [`ParserSettings`](../parsersettings) クラスの新しいインスタンスをロガーと共に初期化します。 |
| [ParserSettings](parsersettings#constructor_4)(OcrConnectorBase) | [`ParserSettings`](../parsersettings) クラスの新しいインスタンスを OCR コネクタと共に初期化します。 |
| [ParserSettings](parsersettings#constructor_2)(ILogger, OcrConnectorBase) | [`ParserSettings`](../parsersettings) クラスの新しいインスタンスをロガーと OCR コネクタと共に初期化します。 |
| [ParserSettings](parsersettings#constructor_3)(ILogger, OcrConnectorBase, ExternalResourceHandler) | [`ParserSettings`](../parsersettings) クラスの新しいインスタンスをロガー、OCR コネクタ、外部リソースハンドラと共に初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [ExternalResourceHandler](../../groupdocs.parser.options/parsersettings/externalresourcehandler) { get; } | 外部リソース用ハンドラを取得します。 |
| [Logger](../../groupdocs.parser.options/parsersettings/logger) { get; } | データ抽出中のイベントやエラーの記録に使用されるロガーを取得します。 |
| [OcrConnector](../../groupdocs.parser.options/parsersettings/ocrconnector) { get; } | OCR 機能を提供するために使用される OCR コネクタを取得します。 |

### 備考

**Learn more:**

* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
