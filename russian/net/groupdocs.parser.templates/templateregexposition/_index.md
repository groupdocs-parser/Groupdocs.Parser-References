---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет позицию поля шаблона, использующую регулярное выражение."
type: docs
weight: 150
url: /ru/net/groupdocs.parser.templates/templateregexposition/
---

## TemplateRegexPosition class

Предоставляет позицию поля шаблона, использующую регулярное выражение.

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | Инициализирует новый экземпляр класса [`TemplateRegexPosition`](../templateregexposition). |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | Инициализирует новый экземпляр класса [`TemplateRegexPosition`](../templateregexposition). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | Возвращает регулярное выражение. |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | Возвращает значение, указывающее, не игнорируется ли регистр текста. |

### Примеры

Следующий пример показывает ситуацию, когда документ содержит "Invoice Number INV-12345", тогда поле шаблона можно определить следующим образом:

```csharp
// Создайте поле шаблона regex с именем "InvoiceNumber"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

В этом случае в качестве значения извлекается вся строка. Чтобы извлечь только часть строки, используется группа регулярного выражения "value":

```csharp
// Создайте поле шаблона regex с именем "InvoiceNumber" с группой "value"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

В этом случае в качестве значения извлекается строка "INV-3337".

### См. также

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
