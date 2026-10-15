---
title: "OcrOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, которые используются для OCR Connector."
type: docs
weight: 450
url: /ru/net/groupdocs.parser.options/ocroptions/
---

## OcrOptions class

Предоставляет параметры, которые используются для OCR Connector.

```csharp
public class OcrOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OcrOptions](ocroptions#constructor)() | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions) с прямоугольной областью. |
| [OcrOptions](ocroptions#constructor_5)(OcrEventHandler) | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions) с объектом [`OcrEventHandler`](../ocreventhandler). |
| [OcrOptions](ocroptions#constructor_6)(PagePreviewOptions) | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions) с прямоугольной областью. |
| [OcrOptions](ocroptions#constructor_1)(Rectangle) | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions) с прямоугольной областью. |
| [OcrOptions](ocroptions#constructor_2)(Rectangle, OcrEventHandler) | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions) с прямоугольной областью и объектом [`OcrEventHandler`](../ocreventhandler). |
| [OcrOptions](ocroptions#constructor_3)(Rectangle, OcrEventHandler, PagePreviewOptions, bool) | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions). |
| [OcrOptions](ocroptions#constructor_4)(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) | Инициализирует новый экземпляр класса [`OcrOptions`](../ocroptions). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Handler](../../groupdocs.parser.options/ocroptions/handler) { get; set; } | Получает обработчик событий для перехвата OCR‑событий. |
| [Language](../../groupdocs.parser.options/ocroptions/language) { get; set; } | Получает или задает язык, используемый для OCR. Определяет алфавит, используемый во время распознавания. По умолчанию используется английский. |
| [PagePreviewOptions](../../groupdocs.parser.options/ocroptions/pagepreviewoptions) { get; set; } | Получает параметры предварительного просмотра страниц документа. |
| [Rectangle](../../groupdocs.parser.options/ocroptions/rectangle) { get; set; } | Получает прямоугольную область, ограничивающую область страницы, используемую для распознавания текста. |
| [UseSpellChecker](../../groupdocs.parser.options/ocroptions/usespellchecker) { get; set; } | Получает значение, указывающее, используется ли проверка орфографии. |

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
