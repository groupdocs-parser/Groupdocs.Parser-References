---
title: TemplateTable
second_title: Справочник по API GroupDocs.Parser для .NET
description: Предоставляет таблицу шаблонов.
type: docs
weight: 740
url: /ru/net/groupdocs.parser.templates/templatetable/
---
## TemplateTable class

Предоставляет таблицу шаблонов.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string, int?) | Инициализирует новый экземпляр[`TemplateTable`](../templatetable) класс. |
| [TemplateTable](templatetable#constructor_1)(TemplateTableParameters, string, int?) | Инициализирует новый экземпляр[`TemplateTable`](../templatetable) класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Получает макет таблицы. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Получает имя элемента шаблона. |
| [PageIndex](../../groupdocs.parser.templates/templateitem/pageindex) { get; } | Получает индекс страницы элемента шаблона. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Получает параметры для обнаружения таблицы в автоматическом режиме. |

### Примечания

Существует два способа определения таблицы:

* Использование[`TemplateTableLayout`](../templatetablelayout) сорт. В этом случае таблица определяется своим положением на странице: прямоугольная область, разделители столбцов и строк.
* Использование[`TemplateTableParameters`](../templatetableparameters) class. В этом случае таблица определяется автоматически алгоритмами с заданными параметрами. См.[`TemplateTableParameters`](../templatetableparameters) класс для получения дополнительной информации.

### Смотрите также

* class [TemplateItem](../templateitem)
* пространство имен [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* сборка [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
