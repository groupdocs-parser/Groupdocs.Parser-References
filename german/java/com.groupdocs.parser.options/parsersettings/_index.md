---
title: "ParserSettings"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Einstellungen bereit, die zur Anpassung der Datenerfassung verwendet werden."
type: docs
weight: 33
url: /de/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Stellt die Einstellungen bereit, die zur Anpassung der Datenerfassung verwendet werden.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit dem Logger. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit dem OCR‑Connector. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit dem External‑Resource‑Handler. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit Logger und OCR‑Connector. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getLogger()](#getLogger--) | Ermittelt den Logger, der für das Protokollieren von Ereignissen und Fehlern während der Datenerfassung verwendet wird. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Ermittelt den OCR‑Connector, der zur Bereitstellung von OCR‑Funktionalität verwendet wird. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Ermittelt den Handler für externe Ressourcen. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit dem Logger.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Eine Instanz einer Klasse, die das Interface [ILogger](../../com.groupdocs.parser.options/ilogger) implementiert. |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit dem OCR‑Connector.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Eine Instanz einer Klasse, die von der Klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erbt, um OCR‑Funktionalität bereitzustellen. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit dem External‑Resource‑Handler.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Eine Instanz einer Klasse, die von der Klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erbt, um OCR‑Funktionalität bereitzustellen. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings) mit Logger und OCR‑Connector.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Eine Instanz einer Klasse, die das Interface [ILogger](../../com.groupdocs.parser.options/ilogger) implementiert. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Eine Instanz einer Klasse, die von der Klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erbt, um OCR‑Funktionalität bereitzustellen. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Initialisiert eine neue Instanz der Klasse [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Eine Instanz einer Klasse, die das Interface [ILogger](../../com.groupdocs.parser.options/ilogger) implementiert. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Eine Instanz einer Klasse, die von der Klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) erbt, um OCR‑Funktionalität bereitzustellen. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Eine Instanz einer Klasse, die von der Klasse [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) erbt, um die Steuerung des Ladens externer Ressourcen zu ermöglichen. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Ermittelt den Logger, der für das Protokollieren von Ereignissen und Fehlern während der Datenerfassung verwendet wird.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Ermittelt den OCR‑Connector, der zur Bereitstellung von OCR‑Funktionalität verwendet wird.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Ermittelt den Handler für externe Ressourcen.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

