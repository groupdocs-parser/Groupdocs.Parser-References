---
title: "DocumentPageData"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет данные страницы документа. Состоит из объектов FieldData./fielddata, содержащих данные полей со страницы документа."
type: docs
weight: 740
url: /ru/net/groupdocs.parser.data/documentpagedata/
---

## DocumentPageData class

Представляет данные страницы документа. Состоит из объектов [`FieldData`](../fielddata), содержащих данные полей со страницы документа.

```csharp
public sealed class DocumentPageData : DocumentData
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Возвращает общее количество данных полей. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Возвращает данные поля по индексу. |
| [PageIndex](../../groupdocs.parser.data/documentpagedata/pageindex) { get; } | Получает индекс страницы. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Возвращает шаблон. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Возвращает перечислитель для данных полей. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Возвращает коллекцию данных полей, где имя равно *fieldName*. |

### См. также

* class [DocumentData](../documentdata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
