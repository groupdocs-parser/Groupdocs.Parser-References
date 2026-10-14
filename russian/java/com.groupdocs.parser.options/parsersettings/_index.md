---
title: "ParserSettings"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет настройки, используемые для настройки извлечения данных."
type: docs
weight: 33
url: /ru/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Предоставляет настройки, используемые для настройки извлечения данных.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с логгером. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с OCR‑коннектором. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с обработчиком внешних ресурсов. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с логгером и OCR‑коннектором. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getLogger()](#getLogger--) | Возвращает логгер, используемый для записи событий и ошибок во время извлечения данных. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Возвращает OCR‑коннектор, используемый для предоставления OCR‑функциональности. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Возвращает обработчик внешних ресурсов. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с логгером.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Экземпляр класса, реализующего интерфейс [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с OCR‑коннектором.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Экземпляр класса, наследующего класс [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) для предоставления OCR‑функциональности. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с обработчиком внешних ресурсов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Экземпляр класса, наследующего класс [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) для предоставления OCR‑функциональности. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings) с логгером и OCR‑коннектором.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Экземпляр класса, реализующего интерфейс [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Экземпляр класса, наследующего класс [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) для предоставления OCR‑функциональности. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Инициализирует новый экземпляр класса [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Экземпляр класса, реализующего интерфейс [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Экземпляр класса, наследующего класс [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) для предоставления OCR‑функциональности. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Экземпляр класса, наследующего класс [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) для контроля загрузки внешних ресурсов. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Возвращает логгер, используемый для записи событий и ошибок во время извлечения данных.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Возвращает OCR‑коннектор, используемый для предоставления OCR‑функциональности.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Возвращает обработчик внешних ресурсов.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

