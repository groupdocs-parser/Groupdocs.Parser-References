---
title: "ParserSettings"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Veri çıkarımını özelleştirmek için kullanılan ayarları sağlar."
type: docs
weight: 33
url: /tr/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Veri çıkarımını özelleştirmek için kullanılan ayarları sağlar.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini logger ile başlatır. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini OCR Bağlayıcısı ile başlatır. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini Harici Kaynak İşleyicisi ile başlatır. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini logger ve OCR Bağlayıcısı ile başlatır. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getLogger()](#getLogger--) | Veri çıkarımı sırasında olayları ve hataları kaydetmek için kullanılan günlüğü alır. |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR işlevselliği sağlamak için kullanılan OCR Bağlayıcısını alır. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Harici kaynaklar için işleyiciyi alır. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini logger ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) arayüzünü uygulayan bir sınıf örneği. |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini OCR Bağlayıcısı ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR işlevselliği sağlamak için [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) sınıfından türetilen bir sınıf örneği. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini Harici Kaynak İşleyicisi ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | OCR işlevselliği sağlamak için [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) sınıfından türetilen bir sınıf örneği. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfı örneğini logger ve OCR Bağlayıcısı ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) arayüzünü uygulayan bir sınıf örneği. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR işlevselliği sağlamak için [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) sınıfından türetilen bir sınıf örneği. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Yeni bir [ParserSettings](../../com.groupdocs.parser.options/parsersettings) sınıfının bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) arayüzünü uygulayan bir sınıf örneği. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR işlevselliği sağlamak için [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) sınıfından türetilen bir sınıf örneği. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Harici kaynak yüklemesini kontrol etmek için [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) sınıfından türetilen bir sınıf örneği. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Veri çıkarımı sırasında olayları ve hataları kaydetmek için kullanılan günlüğü alır.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


OCR işlevselliği sağlamak için kullanılan OCR Bağlayıcısını alır.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Harici kaynaklar için işleyiciyi alır.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

