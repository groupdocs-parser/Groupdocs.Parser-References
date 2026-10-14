---
title: "ParserSettings"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona la configuración que se utiliza para personalizar la extracción de datos."
type: docs
weight: 33
url: /es/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Proporciona la configuración que se utiliza para personalizar la extracción de datos.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el registrador. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el Conector OCR. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el Manejador de Recursos Externos. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el registrador y el Conector OCR. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getLogger()](#getLogger--) | Obtiene el registrador que se utiliza para registrar eventos y errores durante la extracción de datos. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtiene el Conector OCR que se utiliza para proporcionar funcionalidad OCR. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Obtiene el manejador para recursos externos. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el registrador.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Una instancia de clase que implementa la interfaz [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el Conector OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Una instancia de clase que hereda de la clase [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) para proporcionar funcionalidad OCR. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el Manejador de Recursos Externos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Una instancia de clase que hereda de la clase [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) para proporcionar funcionalidad OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings) con el registrador y el Conector OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Una instancia de clase que implementa la interfaz [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Una instancia de clase que hereda de la clase [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) para proporcionar funcionalidad OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Inicializa una nueva instancia de la clase [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Una instancia de clase que implementa la interfaz [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Una instancia de clase que hereda de la clase [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) para proporcionar funcionalidad OCR. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Una instancia de clase que hereda de la clase [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) para proporcionar el control de la carga de recursos externos. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Obtiene el registrador que se utiliza para registrar eventos y errores durante la extracción de datos.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Obtiene el Conector OCR que se utiliza para proporcionar funcionalidad OCR.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Obtiene el manejador para recursos externos.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

