---
title: "ParserSettings"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ParserSettingsgroupdocs.parser.options/parsersettings クラスの新しいインスタンスをロガーとともに初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/parsersettings/parsersettings/
---

## ParserSettings(ILogger) {#constructor_1}

[`ParserSettings`](../../parsersettings) クラスの新しいインスタンスをロガーとともに初期化します。

```csharp
public ParserSettings(ILogger logger)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| logger | ILogger | [`ILogger`](../../ilogger) インターフェイスを実装したクラスのインスタンスです。 |

### 関連項目

* interface [ILogger](../../ilogger)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(OcrConnectorBase) {#constructor_4}

[`ParserSettings`](../../parsersettings) クラスの新しいインスタンスを OCR コネクタとともに初期化します。

```csharp
public ParserSettings(OcrConnectorBase ocrConnector)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ocrConnector | OcrConnectorBase | OCR 機能を提供するために [`OcrConnectorBase`](../../ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |

### 関連項目

* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ExternalResourceHandler) {#constructor}

[`ParserSettings`](../../parsersettings) クラスの新しいインスタンスを外部リソースハンドラとともに初期化します。

```csharp
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| externalResourceHandler | ExternalResourceHandler | 外部リソースのロード制御を提供するために [`ExternalResourceHandler`](../../externalresourcehandler) クラスを継承したクラスのインスタンスです。 |

### 関連項目

* class [ExternalResourceHandler](../../externalresourcehandler)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase) {#constructor_2}

[`ParserSettings`](../../parsersettings) クラスの新しいインスタンスをロガーと OCR コネクタとともに初期化します。

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| logger | ILogger | [`ILogger`](../../ilogger) インターフェイスを実装したクラスのインスタンスです。 |
| ocrConnector | OcrConnectorBase | OCR 機能を提供するために [`OcrConnectorBase`](../../ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |

### 関連項目

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase, ExternalResourceHandler) {#constructor_3}

`[`ParserSettings`](../../parsersettings)` クラスの新しいインスタンスを初期化し、ロガー、OCR コネクタ、外部リソースハンドラを設定します。

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, 
    ExternalResourceHandler externalResourceHandler)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| logger | ILogger | [`ILogger`](../../ilogger) インターフェイスを実装したクラスのインスタンスです。 |
| ocrConnector | OcrConnectorBase | OCR 機能を提供するために [`OcrConnectorBase`](../../ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |
| externalResourceHandler | ExternalResourceHandler | `[`ExternalResourceHandler`](../../externalresourcehandler)` クラスを継承したクラスのインスタンスで、外部リソースのロード制御を提供します。 |

### 関連項目

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ExternalResourceHandler](../../externalresourcehandler)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
