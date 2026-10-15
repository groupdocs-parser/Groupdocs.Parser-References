---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет позицию поля шаблона, использующую связанное поле."
type: docs
weight: 110
url: /ru/net/groupdocs.parser.templates/templatelinkedposition/
---

## TemplateLinkedPosition class

Предоставляет позицию поля шаблона, использующую связанное поле.

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | Инициализирует новый экземпляр класса [`TemplateLinkedPosition`](../templatelinkedposition). |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | Инициализирует новый экземпляр класса [`TemplateLinkedPosition`](../templatelinkedposition) с именем связанного поля в верхнем регистре. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_2)(string, Size, TemplateLinkedPositionEdges, bool, bool) | Инициализирует новый экземпляр класса [`TemplateLinkedPosition`](../templatelinkedposition). |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | Получает значение, указывающее, масштабируется ли [`SearchArea`](./searcharea) по размеру связанного поля. |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | Получает границы связанного поля, в котором производится поиск. |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | Получает имя связанного поля. |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | Получает размер области, в которой производится поиск поля. |

### Примеры

Следующий пример показывает код для ситуации, когда известно, что поле с номером счета размещено справа от строки "Invoice number", используется следующий код:

```csharp
// Создайте шаблонное поле с регулярным выражением для поиска текста "Invoice Number"
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// Создайте связанное шаблонное поле, ассоциированное с полем "Invoice", и извлеките значение, расположенное справа от него
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### См. также

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
