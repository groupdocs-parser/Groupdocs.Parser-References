---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры для алгоритмов обнаружения таблиц."
type: docs
weight: 180
url: /ru/net/groupdocs.parser.templates/templatetableparameters/
---

## TemplateTableParameters class

Предоставляет параметры для алгоритмов обнаружения таблиц.

```csharp
public sealed class TemplateTableParameters
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Инициализирует новый экземпляр класса [`TemplateTableParameters`](../templatetableparameters). |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Инициализирует новый экземпляр класса [`TemplateTableParameters`](../templatetableparameters). |

## Свойства

| Имя | Описание |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Получает значение, указывающее, содержит ли таблица объединённые ячейки. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Получает минимальное количество столбцов таблицы. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Получает минимальное количество строк таблицы. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Получает минимальное расстояние между столбцами таблицы. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Получает прямоугольную область, содержащую таблицу. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Получает разделители столбцов таблицы. |

### Примечания

Существует два алгоритма обнаружения таблицы:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

В некоторых случаях, когда алгоритмы не могут обнаружить таблицу или делают это неточно, используется класс [`TemplateTableLayout`](../templatetablelayout).

### См. также

* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
