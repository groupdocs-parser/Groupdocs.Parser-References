---
title: "Шаблон"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет шаблон страницы документа. Он состоит из объектов TemplateItem./templateitem, которые представляют элементы шаблона, такие как текстовые поля и определения таблиц."
type: docs
weight: 50
url: /ru/net/groupdocs.parser.templates/template/
---

## Template class

Предоставляет шаблон страницы документа. Он состоит из объектов [`TemplateItem`](../templateitem), которые представляют элементы шаблона, такие как текстовые поля и определения таблиц.

```csharp
public sealed class Template : IEnumerable<TemplateItem>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Template](template#constructor)(IEnumerable&lt;TemplateItem&gt;) | Инициализирует новый экземпляр класса [`Template`](../template). |
| [Template](template#constructor_1)(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) | Инициализирует новый экземпляр класса [`Template`](../template) с параметрами шаблона. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../groupdocs.parser.templates/template/count) { get; } | Получает общее количество элементов шаблона. |
| [IsOcrCompatible](../../groupdocs.parser.templates/template/isocrcompatible) { get; } | Получает значение, указывающее, совместим ли шаблон с OCR. |
| [Item](../../groupdocs.parser.templates/template/item) { get; } | Получает элемент шаблона по индексу. |
| [Options](../../groupdocs.parser.templates/template/options) { get; } | Получает параметры шаблона. |

## Методы

| Имя | Описание |
| --- | --- |
| static [Load](../../groupdocs.parser.templates/template/load#load)(Stream) | Загружает шаблон из потока. |
| static [Load](../../groupdocs.parser.templates/template/load#load_1)(string) | Загружает шаблон из файла. |
| [GetEnumerator](../../groupdocs.parser.templates/template/getenumerator)() | Возвращает перечислитель для элементов шаблона. |
| [Save](../../groupdocs.parser.templates/template/save#save)(Stream) | Сохраняет шаблон в поток. |
| [Save](../../groupdocs.parser.templates/template/save#save_1)(string) | Сохраняет шаблон в файл. |

### Примечания

**Learn more:**

* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)

### См. также

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
