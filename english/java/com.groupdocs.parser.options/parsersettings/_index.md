---
title: ParserSettings
second_title: GroupDocs.Parser for Java API Reference
description: Provides the settings which are used to customize data extraction.
type: docs
weight: 32
url: /java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Provides the settings which are used to customize data extraction.

**Learn more:**

 *  [Logging][]


[Logging]: https://docs.groupdocs.com/display/parserjava/Logging
## Constructors

| Constructor | Description |
| --- | --- |
| [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with the logger. |
| [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with the OCR Connector. |
| [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with the External Resource Handler. |
| [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with logger and OCR Connector. |
| [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLogger()](#getLogger--) | Gets the logger which is used for logging events and errors during data extraction. |
| [getOcrConnector()](#getOcrConnector--) | Gets the OCR Connector which is used to provide OCR functionality. |
| [getExternalResourceHandler()](#getExternalResourceHandler--) | Gets the handler for external resources. |
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with the logger.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface. |

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with the OCR Connector.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with the External Resource Handler.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class with logger and OCR Connector.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface. |
| ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Initializes a new instance of the [ParserSettings](../../com.groupdocs.parser.options/parsersettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface. |
| ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |
| externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading. |

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Gets the logger which is used for logging events and errors during data extraction.

**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.
### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Gets the OCR Connector which is used to provide OCR functionality.

**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.
### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Gets the handler for external resources.

**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.
