---
title: "WorksheetInfo"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Создаёт новый экземпляр класса WorksheetInfogroupdocs.parser.data/worksheetinfo."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---

## WorksheetInfo constructor

Создаёт новый экземпляр класса [`WorksheetInfo`](../../worksheetinfo).

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Нулевой индекс листа. |
| имя | Строка | Строковое значение, представляющее имя листа. |
| range | WorksheetRange | Экземпляр класса [`WorksheetRange`](../../worksheetrange), представляющий размер листа. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Индекс листа не может быть отрицательным. |
| ArgumentNullException | Размер листа не может быть `null`. |

### См. также

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
