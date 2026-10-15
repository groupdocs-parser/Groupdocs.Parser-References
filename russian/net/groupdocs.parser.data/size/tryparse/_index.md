---
title: "TryParse"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Преобразует строковое представление размера в его эквивалент класса. Возвращаемое значение указывает, удалось ли преобразование или нет."
type: docs
weight: 70
url: /ru/net/groupdocs.parser.data/size/tryparse/
---

## Size.TryParse method

Преобразует строковое представление размера в его эквивалент класса. Возвращаемое значение указывает, удалось ли преобразование или нет.

```csharp
public static bool TryParse(string s, out Size size)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| s | Строка | Строка, содержащая размер для преобразования. |
| size | Size& | После возврата метода он содержит экземпляр класса [`Size`](../../size), эквивалентный значению, указанному в параметре *s*, если преобразование удалось; иначе `null`. |

### Возвращаемое значение

`true`, если *s* успешно преобразован; иначе, `false`.

### См. также

* class [Size](../../size)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
