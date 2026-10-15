---
title: "TemplateTable"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет таблицу шаблона."
type: docs
weight: 160
url: /ru/net/groupdocs.parser.templates/templatetable/
---

## TemplateTable class

Предоставляет таблицу шаблона.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string) | Инициализирует новый экземпляр класса [`TemplateTable`](../templatetable) с именем в верхнем регистре. |
| [TemplateTable](templatetable#constructor_3)(TemplateTableParameters, string) | Инициализирует новый экземпляр класса [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_1)(TemplateTableLayout, string, double?) | Инициализирует новый экземпляр класса [`TemplateTable`](../templatetable) с именем в верхнем регистре. |
| [TemplateTable](templatetable#constructor_4)(TemplateTableParameters, string, double?) | Инициализирует новый экземпляр класса [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_2)(TemplateTableLayout, string, double?, bool) | Инициализирует новый экземпляр класса [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_5)(TemplateTableParameters, string, double?, bool) | Инициализирует новый экземпляр класса [`TemplateTable`](../templatetable). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Получает макет таблицы. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Получает имя элемента шаблона. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Получает ширину страницы, использованной для создания элемента шаблона. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Получает параметры для обнаружения таблицы в автоматическом режиме. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Получает логическое значение, указывающее, был ли `Name` преобразован в ВЕРХНИЙ РЕГИСТР. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatetable/scale)(double) | Масштабирует этот элемент шаблона на заданный коэффициент. |

### Примечания

Существует два способа определения таблицы:

* Using [`TemplateTableLayout`](../templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [`TemplateTableParameters`](../templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](../templatetableparameters) class for more information.

### См. также

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
