---
title: "ParserSettings"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les paramètres utilisés pour personnaliser l'extraction de données."
type: docs
weight: 33
url: /fr/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Fournit les paramètres utilisés pour personnaliser l'extraction de données.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le logger. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le connecteur OCR. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le gestionnaire de ressources externes. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le logger et le connecteur OCR. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getLogger()](#getLogger--) | Obtient le logger qui est utilisé pour consigner les événements et les erreurs lors de l'extraction des données. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtient le connecteur OCR qui est utilisé pour fournir la fonctionnalité OCR. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Obtient le gestionnaire des ressources externes. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le logger.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Une instance de classe qui implémente l'interface [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le connecteur OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Une instance de classe qui hérite de la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) pour fournir la fonctionnalité OCR. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le gestionnaire de ressources externes.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Une instance de classe qui hérite de la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) pour fournir la fonctionnalité OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) avec le logger et le connecteur OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Une instance de classe qui implémente l'interface [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Une instance de classe qui hérite de la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) pour fournir la fonctionnalité OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Initialise une nouvelle instance de la classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Une instance de classe qui implémente l'interface [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Une instance de classe qui hérite de la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) pour fournir la fonctionnalité OCR. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Une instance de classe qui hérite de la classe [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) pour fournir le contrôle du chargement des ressources externes. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Obtient le logger qui est utilisé pour consigner les événements et les erreurs lors de l'extraction des données.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Obtient le connecteur OCR qui est utilisé pour fournir la fonctionnalité OCR.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Obtient le gestionnaire des ressources externes.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

