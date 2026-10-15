---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет информацию о том, как отображается страница."
type: docs
weight: 500
url: /ru/net/groupdocs.parser.options/pagerenderinfo/
---

## PageRenderInfo class

Представляет информацию о том, как отображается страница.

```csharp
public sealed class PageRenderInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageRenderInfo](pagerenderinfo)(int, int, int) | Инициализирует новый экземпляр класса [`PageRenderInfo`](../pagerenderinfo). |

## Свойства

| Имя | Описание |
| --- | --- |
| [ColumnCount](../../groupdocs.parser.options/pagerenderinfo/columncount) { get; } | Получить общее количество столбцов плиток. |
| [PageNumber](../../groupdocs.parser.options/pagerenderinfo/pagenumber) { get; } | Получает номер страницы. |
| [RowCount](../../groupdocs.parser.options/pagerenderinfo/rowcount) { get; } | Получить общее количество строк плиток. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetColumn](../../groupdocs.parser.options/pagerenderinfo/getcolumn)(int) | Возвращает индекс столбца, в котором размещена плитка с *tileIndex*. |
| [GetRow](../../groupdocs.parser.options/pagerenderinfo/getrow)(int) | Возвращает индекс строки, в которой размещена плитка с *tileIndex*. |

### Примечания

Некоторые документы (например, электронные таблицы) невозможно отобразить страницу в виде одного изображения. Для таких документов страница рендерится как набор плиток. Эти плитки размещаются в прямоугольной таблице.

[`RowCount`](./rowcount) and [`ColumnCount`](./columncount) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
