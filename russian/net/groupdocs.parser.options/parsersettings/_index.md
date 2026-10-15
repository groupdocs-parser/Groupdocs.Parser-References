---
title: "ParserSettings"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет настройки, используемые для настройки извлечения данных."
type: docs
weight: 540
url: /ru/net/groupdocs.parser.options/parsersettings/
---

## ParserSettings class

Предоставляет настройки, используемые для настройки извлечения данных.

```csharp
public sealed class ParserSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ParserSettings](parsersettings#constructor)(ExternalResourceHandler) | Инициализирует новый экземпляр класса [`ParserSettings`](../parsersettings) с обработчиком внешних ресурсов. |
| [ParserSettings](parsersettings#constructor_1)(ILogger) | Инициализирует новый экземпляр класса [`ParserSettings`](../parsersettings) с логгером. |
| [ParserSettings](parsersettings#constructor_4)(OcrConnectorBase) | Инициализирует новый экземпляр класса [`ParserSettings`](../parsersettings) с OCR Connector. |
| [ParserSettings](parsersettings#constructor_2)(ILogger, OcrConnectorBase) | Инициализирует новый экземпляр класса [`ParserSettings`](../parsersettings) с логгером и OCR Connector. |
| [ParserSettings](parsersettings#constructor_3)(ILogger, OcrConnectorBase, ExternalResourceHandler) | Инициализирует новый экземпляр класса [`ParserSettings`](../parsersettings) с логгером, OCR Connector и обработчиком внешних ресурсов. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ExternalResourceHandler](../../groupdocs.parser.options/parsersettings/externalresourcehandler) { get; } | Возвращает обработчик внешних ресурсов. |
| [Logger](../../groupdocs.parser.options/parsersettings/logger) { get; } | Возвращает логгер, используемый для записи событий и ошибок во время извлечения данных. |
| [OcrConnector](../../groupdocs.parser.options/parsersettings/ocrconnector) { get; } | Возвращает OCR Connector, используемый для предоставления функциональности OCR. |

### Примечания

**Learn more:**

* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
