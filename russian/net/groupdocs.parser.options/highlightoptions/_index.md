---
title: "HighlightOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, которые используются для извлечения выделения блока текста вокруг найденного текста в сценариях поиска."
type: docs
weight: 360
url: /ru/net/groupdocs.parser.options/highlightoptions/
---

## HighlightOptions class

Предоставляет параметры, которые используются для извлечения выделения (блока текста вокруг найденного текста в сценариях поиска).

```csharp
public sealed class HighlightOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)() | Инициализирует новый экземпляр класса [`HighlightOptions`](../highlightoptions), который используется для извлечения выделения фиксированной длины. |
| [HighlightOptions](highlightoptions#constructor_1)(int) | Инициализирует новый экземпляр класса [`HighlightOptions`](../highlightoptions), который используется для извлечения выделения фиксированной длины. |
| [HighlightOptions](highlightoptions#constructor_2)(int?, bool) | Инициализирует новый экземпляр класса [`HighlightOptions`](../highlightoptions), который используется для извлечения выделения, ограниченного строкой. |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int) | Инициализирует новый экземпляр класса [`HighlightOptions`](../highlightoptions), который используется для извлечения выделения с фиксированным количеством слов. |
| [HighlightOptions](highlightoptions#constructor_4)(int?, int?, bool) | Инициализирует новый экземпляр класса [`HighlightOptions`](../highlightoptions). |

## Свойства

| Имя | Описание |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; set; } | Получает значение, указывающее, ограничено ли извлечение выделения началом (или концом) строки текста. |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; set; } | Получает максимальную длину текста. |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; set; } | Получает максимальное количество слов. |

### Примечания

Экземпляр класса [`HighlightOptions`](../highlightoptions) используется в качестве параметра метода [`GetHighlight`](../../groupdocs.parser/parser/gethighlight). См. примеры использования там.

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
