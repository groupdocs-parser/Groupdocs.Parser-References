---
title: "ParserSettings"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller inställningarna som används för att anpassa datautvinning."
type: docs
weight: 33
url: /sv/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Tillhandahåller inställningarna som används för att anpassa datautvinning.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med loggaren. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med OCR-anslutningen. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med den externa resurs‑hanteraren. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med loggaren och OCR‑anslutningen. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getLogger()](#getLogger--) | Hämtar loggaren som används för att logga händelser och fel under datautvinning. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Hämtar OCR‑anslutningen som används för att tillhandahålla OCR‑funktionalitet. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Hämtar hanteraren för externa resurser. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med loggaren.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | En instans av en klass som implementerar gränssnittet [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med OCR-anslutningen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | En instans av en klass som ärver klassen [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) för att tillhandahålla OCR‑funktionalitet. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med den externa resurs‑hanteraren.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | En instans av en klass som ärver klassen [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) för att tillhandahålla OCR‑funktionalitet. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings) med loggaren och OCR‑anslutningen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | En instans av en klass som implementerar gränssnittet [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | En instans av en klass som ärver klassen [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) för att tillhandahålla OCR‑funktionalitet. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Initierar en ny instans av klassen [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | En instans av en klass som implementerar gränssnittet [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | En instans av en klass som ärver klassen [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) för att tillhandahålla OCR‑funktionalitet. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | En instans av en klass som ärver klassen [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) för att ge kontroll över inläsning av externa resurser. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Hämtar loggaren som används för att logga händelser och fel under datautvinning.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Hämtar OCR‑anslutningen som används för att tillhandahålla OCR‑funktionalitet.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Hämtar hanteraren för externa resurser.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

