---
title: "PageTableArea"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет область таблицы на странице, используемую для представления таблицы в функции парсинга по шаблону."
type: docs
weight: 840
url: /ru/net/groupdocs.parser.data/pagetablearea/
---

## PageTableArea class

Представляет область таблицы на странице, используемую для представления таблицы в функции парсинга по шаблону.

```csharp
public sealed class PageTableArea : PageArea
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Cells](../../groupdocs.parser.data/pagetablearea/cells) { get; } | Получает коллекцию ячеек. |
| [ColumnCount](../../groupdocs.parser.data/pagetablearea/columncount) { get; } | Получает общее количество столбцов таблицы. |
| [Item](../../groupdocs.parser.data/pagetablearea/item) { get; } | Получает ячейку таблицы по индексам строки и столбца. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Возвращает информацию о странице документа, такую как индекс страницы и её размер. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Получает прямоугольную область. |
| [RowCount](../../groupdocs.parser.data/pagetablearea/rowcount) { get; } | Получает общее количество строк таблицы. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetColumnWidth](../../groupdocs.parser.data/pagetablearea/getcolumnwidth)(int) | Возвращает ширину столбца. |
| [GetRowHeight](../../groupdocs.parser.data/pagetablearea/getrowheight)(int) | Возвращает высоту строки. |

### Примечания

[`PageTableArea`](../pagetablearea) class is used to organize inheritors of [`PageArea`](../pagearea) class in table structure.

### См. также

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
