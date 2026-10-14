---
title: "ParserSettings"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de instellingen die worden gebruikt om gegevensextractie aan te passen."
type: docs
weight: 33
url: /nl/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Biedt de instellingen die worden gebruikt om gegevensextractie aan te passen.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met de logger. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met de OCR-connector. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met de externe resourcehandler. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met logger en OCR-connector. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getLogger()](#getLogger--) | Haalt de logger op die wordt gebruikt voor het loggen van gebeurtenissen en fouten tijdens data-extractie. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Haalt de OCR-connector op die wordt gebruikt om OCR-functionaliteit te bieden. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Haalt de handler voor externe resources op. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met de logger.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Een exemplaar van een klasse die de interface [ILogger](../../com.groupdocs.parser.options/ilogger) implementeert. |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met de OCR-connector.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Een exemplaar van een klasse die de klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erft om OCR-functionaliteit te bieden. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met de externe resourcehandler.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Een exemplaar van een klasse die de klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erft om OCR-functionaliteit te bieden. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) met logger en OCR-connector.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Een exemplaar van een klasse die de interface [ILogger](../../com.groupdocs.parser.options/ilogger) implementeert. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Een exemplaar van een klasse die de klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erft om OCR-functionaliteit te bieden. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Initialiseert een nieuw exemplaar van de klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Een exemplaar van een klasse die de interface [ILogger](../../com.groupdocs.parser.options/ilogger) implementeert. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Een exemplaar van een klasse die de klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erft om OCR-functionaliteit te bieden. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Een exemplaar van een klasse die de klasse [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) erft om de controle over het laden van externe resources te bieden. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Haalt de logger op die wordt gebruikt voor het loggen van gebeurtenissen en fouten tijdens data-extractie.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Haalt de OCR-connector op die wordt gebruikt om OCR-functionaliteit te bieden.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Haalt de handler voor externe resources op.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

