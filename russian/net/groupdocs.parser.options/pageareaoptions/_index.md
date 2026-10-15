---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, которые используются для извлечения областей страниц."
type: docs
weight: 460
url: /ru/net/groupdocs.parser.options/pageareaoptions/
---

## PageAreaOptions class

Предоставляет параметры, которые используются для извлечения областей страниц.

```csharp
public class PageAreaOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageAreaOptions](pageareaoptions#constructor)() | Инициализирует новый экземпляр класса [`PageAreaOptions`](../pageareaoptions). |
| [PageAreaOptions](pageareaoptions#constructor_1)(Rectangle) | Инициализирует новый экземпляр класса [`PageAreaOptions`](../pageareaoptions). |
| [PageAreaOptions](pageareaoptions#constructor_2)(Rectangle, double) | Инициализирует новый экземпляр класса [`PageAreaOptions`](../pageareaoptions) с размером игнорируемой границы. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Получает прямоугольную область, содержащую области страниц. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Получает размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |

### Примечания

Экземпляр класса [`PageAreaOptions`](../pageareaoptions) используется в качестве параметра в следующих методах:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)

Смотрите примеры использования там.

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
