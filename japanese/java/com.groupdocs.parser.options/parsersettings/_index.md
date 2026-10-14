---
title: "ParserSettings"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "データ抽出をカスタマイズするために使用される設定を提供します。"
type: docs
weight: 33
url: /ja/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

データ抽出をカスタマイズするために使用される設定を提供します。

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | ロガーを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。 |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | OCR コネクタを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。 |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | 外部リソースハンドラを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。 |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | ロガーと OCR コネクタを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。 |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | 新しい [ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getLogger()](#getLogger--) | データ抽出中のイベントとエラーのログ記録に使用されるロガーを取得します。 |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR 機能を提供するために使用される OCR コネクタを取得します。 |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | 外部リソース用のハンドラを取得します。 |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


ロガーを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) インターフェイスを実装するクラスのインスタンスです。 |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


OCR コネクタを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR 機能を提供するために [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


外部リソースハンドラを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | OCR 機能を提供するために [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


ロガーと OCR コネクタを使用して、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) インターフェイスを実装するクラスのインスタンスです。 |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR 機能を提供するために [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


新しい [ParserSettings](../../com.groupdocs.parser.options/parsersettings) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) インターフェイスを実装するクラスのインスタンスです。 |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR 機能を提供するために [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) クラスを継承したクラスのインスタンスです。 |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | 外部リソースの読み込み制御を提供するために [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) クラスを継承したクラスのインスタンスです。 |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


データ抽出中のイベントとエラーのログ記録に使用されるロガーを取得します。


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


OCR 機能を提供するために使用される OCR コネクタを取得します。


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


外部リソース用のハンドラを取得します。


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

