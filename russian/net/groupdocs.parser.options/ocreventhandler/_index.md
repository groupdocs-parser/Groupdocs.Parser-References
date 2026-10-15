---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет обработчик событий OCR."
type: docs
weight: 440
url: /ru/net/groupdocs.parser.options/ocreventhandler/
---

## OcrEventHandler class

Предоставляет обработчик событий OCR.

```csharp
public class OcrEventHandler
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OcrEventHandler](ocreventhandler)() | Инициализирует новый экземпляр класса [`OcrEventHandler`](../ocreventhandler). |

## Свойства

| Имя | Описание |
| --- | --- |
| [HasWarnings](../../groupdocs.parser.options/ocreventhandler/haswarnings) { get; } | Возвращает значение, указывающее, не пустой ли список предупреждений. |
| [Warnings](../../groupdocs.parser.options/ocreventhandler/warnings) { get; } | Возвращает список сообщений предупреждений. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetWarnings](../../groupdocs.parser.options/ocreventhandler/getwarnings)(int) | Возвращает список сообщений предупреждений для страницы с *pageIndex*. |
| virtual [OnWarnings](../../groupdocs.parser.options/ocreventhandler/onwarnings)(int, IList&lt;string&gt;) | Устанавливает сообщения предупреждений для страницы. |

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
