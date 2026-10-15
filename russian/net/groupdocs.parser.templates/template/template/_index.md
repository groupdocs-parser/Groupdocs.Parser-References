---
title: "Шаблон"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса Templategroupdocs.parser.templates/template."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.templates/template/template/
---

## Template(IEnumerable&lt;TemplateItem&gt;) {#constructor}

Инициализирует новый экземпляр класса [`Template`](../../template).

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| items | IEnumerable`1 | Коллекция объектов [`TemplateItem`](../../templateitem). |

### Примеры

Использование:

```csharp
// Создайте массив полей шаблона
TemplateItem[] fields = new TemplateItem[]
{
   new TemplateField(new TemplateRegexPosition("From"), "From", 0),
   new TemplateField(
       new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromCompany",
       0),
   new TemplateField(
       new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromAddress",
       0)
};

// Создать шаблон документа
Template template = new Template(fields);
```

### См. также

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Template(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) {#constructor_1}

Инициализирует новый экземпляр класса [`Template`](../../template) с параметрами шаблона.

```csharp
public Template(IEnumerable<TemplateItem> items, TemplateOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| items | IEnumerable`1 | Коллекция объектов [`TemplateItem`](../../templateitem). |
| options | TemplateOptions | Параметры шаблона. |

### См. также

* class [TemplateItem](../../templateitem)
* class [TemplateOptions](../../templateoptions)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
