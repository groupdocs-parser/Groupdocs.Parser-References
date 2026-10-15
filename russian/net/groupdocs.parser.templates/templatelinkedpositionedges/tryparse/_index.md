---
title: "TryParse"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Преобразует строковое представление границ в эквивалентный объект класса. Возвращаемое значение указывает, успешно ли выполнено преобразование или нет."
type: docs
weight: 90
url: /ru/net/groupdocs.parser.templates/templatelinkedpositionedges/tryparse/
---

## TemplateLinkedPositionEdges.TryParse method

Преобразует строковое представление границ в эквивалентный объект класса. Возвращаемое значение указывает, успешно ли выполнено преобразование или нет.

```csharp
public static bool TryParse(string s, out TemplateLinkedPositionEdges edges)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| s | Строка | Строка, содержащая ребра для преобразования. |
| edges | TemplateLinkedPositionEdges& | При возврате метода он содержит экземпляр класса [`TemplateLinkedPositionEdges`](../../templatelinkedpositionedges), эквивалентный значению, указанному в параметре *s*, если преобразование удалось; в противном случае `null`. |

### Возвращаемое значение

`true`, если *s* успешно преобразован; иначе, `false`.

### См. также

* class [TemplateLinkedPositionEdges](../../templatelinkedpositionedges)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
