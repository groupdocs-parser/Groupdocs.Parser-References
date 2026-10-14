---
title: "ParserSettings"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于自定义数据提取的设置。"
type: docs
weight: 33
url: /zh/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

提供用于自定义数据提取的设置。

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | 使用日志记录器初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。 |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | 使用 OCR 连接器初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。 |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | 使用外部资源处理程序初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。 |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | 使用日志记录器和 OCR 连接器初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。 |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | 初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getLogger()](#getLogger--) | 获取用于在数据提取期间记录事件和错误的日志记录器。 |
|
|  | [getOcrConnector()](#getOcrConnector--) | 获取用于提供 OCR 功能的 OCR 连接器。 |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | 获取外部资源的处理程序。 |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


使用日志记录器初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | 实现 [ILogger](../../com.groupdocs.parser.options/ilogger) 接口的类的实例。 |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


使用 OCR 连接器初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | 继承 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 类以提供 OCR 功能的类的实例。 |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


使用外部资源处理程序初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | 继承 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 类以提供 OCR 功能的类的实例。 |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


使用日志记录器和 OCR 连接器初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | 实现 [ILogger](../../com.groupdocs.parser.options/ilogger) 接口的类的实例。 |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | 继承 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 类以提供 OCR 功能的类的实例。 |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


初始化 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | 实现 [ILogger](../../com.groupdocs.parser.options/ilogger) 接口的类的实例。 |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | 继承 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 类以提供 OCR 功能的类的实例。 |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | 继承 [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) 类以控制外部资源加载的类的实例。 |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


获取用于在数据提取期间记录事件和错误的日志记录器。


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


获取用于提供 OCR 功能的 OCR 连接器。


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


获取外部资源的处理程序。


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

