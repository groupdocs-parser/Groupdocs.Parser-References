---
title: "TemplateField"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет текстовое поле шаблона."
type: docs
weight: 80
url: /ru/net/groupdocs.parser.templates/templatefield/
---

## TemplateField class

Предоставляет текстовое поле шаблона.

```csharp
public sealed class TemplateField : TemplateItem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | Инициализирует новый экземпляр класса [`TemplateField`](../templatefield). |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, double?) | Инициализирует новый экземпляр класса [`TemplateField`](../templatefield). |
| [TemplateField](templatefield#constructor_2)(TemplatePosition, string, double?, bool) | Инициализирует новый экземпляр класса [`TemplateField`](../templatefield). |

## Свойства

| Имя | Описание |
| --- | --- |
| [IsHidden](../../groupdocs.parser.templates/templatefield/ishidden) { get; set; } | Получает или задает флаг скрытого поля шаблона. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Получает имя элемента шаблона. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Получает ширину страницы, использованной для создания элемента шаблона. |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | Получает значение, описывающее, как найти поле шаблона на странице документа. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Получает логическое значение, указывающее, был ли `Name` преобразован в ВЕРХНИЙ РЕГИСТР. |
| [Value](../../groupdocs.parser.templates/templatefield/value) { get; set; } | Получает или задает значение поля шаблона. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatefield/scale)(double) | Масштабирует этот элемент шаблона на заданный коэффициент. |

### Примечания

Текстовые поля определяются их положением на странице. Существует три способа определить текстовое поле:

* [`Using the rectangular area`](../templatefixedposition)
* [`Using the regular expression`](../templateregexposition)
* [`Using the linked field`](../templatelinkedposition)

### См. также

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
