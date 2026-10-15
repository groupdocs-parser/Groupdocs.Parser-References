---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, используемые для извлечения областей текста страниц."
type: docs
weight: 520
url: /ru/net/groupdocs.parser.options/pagetextareaoptions/
---

## PageTextAreaOptions class

Предоставляет параметры, используемые для извлечения областей текста страниц.

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)() | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с параметром использования OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с параметром использования OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с регулярным выражением. Другие параметры устанавливаются по умолчанию (см. примечания для деталей). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(bool, OcrOptions) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с возможностью задавать параметры OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_6)(string, Rectangle) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с регулярным выражением и прямоугольной областью. Другие параметры устанавливаются по умолчанию (см. примечания для деталей). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_7)(string, Rectangle, double) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с регулярным выражением, прямоугольной областью и размером игнорируемой границы. Другие параметры устанавливаются по умолчанию (см. примечания для деталей). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, bool, bool, bool, Rectangle) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_5)(string, bool, bool, bool, Rectangle, double) | Инициализирует новый экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) с размером игнорируемой границы. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; set; } | Возвращает регулярное выражение. |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; set; } | Возвращает значение, указывающее, игнорируется ли форматирование текста. |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; set; } | Возвращает значение, указывающее, не игнорируется ли регистр текста. |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; set; } | Возвращает дополнительные параметры для функциональности OCR. |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Получает прямоугольную область, содержащую области страниц. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Получает размер границы, игнорируемой при захвате прямоугольной областью. Он измеряется как доля высоты текстового элемента. |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; set; } | Возвращает значение, указывающее, объединены ли сегменты. |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; set; } | Возвращает значение, указывающее, используется ли функциональность OCR для извлечения текстовых областей. |

### Примечания

Экземпляр класса [`PageTextAreaOptions`](../pagetextareaoptions) используется в качестве параметра методов [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) и [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas). См. примеры использования там. **Узнать больше:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### См. также

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
