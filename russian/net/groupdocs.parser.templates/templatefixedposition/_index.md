---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет позицию поля шаблона, определяемую прямоугольной областью."
type: docs
weight: 90
url: /ru/net/groupdocs.parser.templates/templatefixedposition/
---

## TemplateFixedPosition class

Предоставляет позицию поля шаблона, определяемую прямоугольной областью.

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | Инициализирует новый экземпляр класса [`TemplateFixedPosition`](../templatefixedposition). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | Получает прямоугольную область, содержащую шаблонное поле. |

### Примеры

Это самый простой способ определения позиции поля. Требуется задать прямоугольную область на странице, ограничивающую значение поля. Весь текст, содержащийся (даже частично) в этой прямоугольной области, будет извлечён как значение:

```csharp
// Создайте фиксированное шаблонное поле с именем "Address", ограниченное прямоугольником в позиции (35, 160) и размером (110, 20)
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### См. также

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
