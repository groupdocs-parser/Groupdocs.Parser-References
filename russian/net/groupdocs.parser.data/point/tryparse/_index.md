---
title: "TryParse"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Преобразует строковое представление точки в её эквивалентный объект класса. Возвращаемое значение указывает, успешно ли выполнено преобразование."
type: docs
weight: 80
url: /ru/net/groupdocs.parser.data/point/tryparse/
---

## Point.TryParse method

Преобразует строковое представление точки в её эквивалентный объект класса. Возвращаемое значение указывает, успешно ли выполнено преобразование.

```csharp
public static bool TryParse(string s, out Point point)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| s | Строка | Строка, содержащая точку для преобразования. |
| point | Point& | Когда метод возвращается, он содержит экземпляр класса [`Point`](../../point), эквивалентный значению, указанному в параметре *s*, если преобразование успешно; иначе `null`. |

### Возвращаемое значение

`true`, если *s* успешно преобразован; иначе, `false`.

### См. также

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
