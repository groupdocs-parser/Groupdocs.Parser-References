---
title: "GetAnnotations"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает аннотации из документа. Обратите внимание, что в настоящее время поддерживается только формат PDF."
type: docs
weight: 60
url: /ru/net/groupdocs.parser/parser/getannotations/
---

## GetAnnotations() {#getannotations}

Извлекает аннотации из документа. Обратите внимание, что в настоящее время поддерживается только формат PDF.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations()
```

### Возвращаемое значение

Коллекция элементов аннотаций; `null`, если извлечение аннотаций не поддерживается.

### См. также

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetAnnotations(int) {#getannotations_1}

Извлекает аннотации со страницы документа. Обратите внимание, что в настоящее время поддерживается только формат PDF.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Коллекция элементов аннотаций; `null`, если извлечение аннотаций не поддерживается.

### См. также

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
