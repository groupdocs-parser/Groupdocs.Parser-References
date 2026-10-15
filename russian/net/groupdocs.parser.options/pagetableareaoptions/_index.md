---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, используемые для извлечения областей таблиц страниц."
type: docs
weight: 510
url: /ru/net/groupdocs.parser.options/pagetableareaoptions/
---

## PageTableAreaOptions class

Предоставляет параметры, используемые для извлечения областей таблиц страниц.

```csharp
public sealed class PageTableAreaOptions : PageAreaOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageTableAreaOptions](pagetableareaoptions)(TemplateTableLayout) | Инициализирует новый экземпляр класса [`PageAreaOptions`](../pageareaoptions). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Получает прямоугольную область, содержащую области страниц. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Получает размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |
| [TableLayout](../../groupdocs.parser.options/pagetableareaoptions/tablelayout) { get; } | Получает макет таблицы, определяющий таблицу на странице. |

### Примечания

Экземпляр класса [`PageTableAreaOptions`](../pagetableareaoptions) используется в качестве параметра методов [`GetTables`](../../groupdocs.parser/parser/gettables) и [`GetTables`](../../groupdocs.parser/parser/gettables). См. примеры использования там.

### См. также

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
