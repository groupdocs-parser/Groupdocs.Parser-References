---
title: "DocumentData"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет данные документа. Состоит из объектов FieldData./fielddata, содержащих данные полей из документа."
type: docs
weight: 730
url: /ru/net/groupdocs.parser.data/documentdata/
---

## DocumentData class

Представляет данные документа. Состоит из объектов [`FieldData`](../fielddata), содержащих данные полей из документа.

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Возвращает общее количество данных полей. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Возвращает данные поля по индексу. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Возвращает шаблон. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Возвращает перечислитель для данных полей. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Возвращает коллекцию данных полей, где имя равно *fieldName*. |

### Примечания

Экземпляр класса [`DocumentData`](../documentdata) используется в качестве возвращаемого значения методов [`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) и [`ParseForm`](../../groupdocs.parser/parser/parseform). См. примеры использования там.

### См. также

* class [FieldData](../fielddata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
