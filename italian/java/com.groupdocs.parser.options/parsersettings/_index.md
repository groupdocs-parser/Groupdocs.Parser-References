---
title: "ParserSettings"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le impostazioni utilizzate per personalizzare l'estrazione dei dati."
type: docs
weight: 33
url: /it/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Fornisce le impostazioni utilizzate per personalizzare l'estrazione dei dati.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il logger. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il connettore OCR. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il gestore delle risorse esterne. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il logger e il connettore OCR. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getLogger()](#getLogger--) | Restituisce il logger utilizzato per registrare eventi ed errori durante l'estrazione dei dati. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Restituisce il connettore OCR utilizzato per fornire la funzionalità OCR. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Restituisce il gestore per le risorse esterne. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il logger.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Un'istanza di classe che implementa l'interfaccia [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il connettore OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Un'istanza di classe che eredita la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) per fornire la funzionalità OCR. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il gestore delle risorse esterne.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Un'istanza di classe che eredita la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) per fornire la funzionalità OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con il logger e il connettore OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Un'istanza di classe che implementa l'interfaccia [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Un'istanza di classe che eredita la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) per fornire la funzionalità OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Inizializza una nuova istanza della classe [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Un'istanza di classe che implementa l'interfaccia [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Un'istanza di classe che eredita la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) per fornire la funzionalità OCR. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Un'istanza di classe che eredita la classe [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) per fornire il controllo del caricamento delle risorse esterne. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Restituisce il logger utilizzato per registrare eventi ed errori durante l'estrazione dei dati.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Restituisce il connettore OCR utilizzato per fornire la funzionalità OCR.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Restituisce il gestore per le risorse esterne.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

