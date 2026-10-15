---
title: "PageTextArea"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет текстовую область страницы, используемую для представления текстового значения в функции парсинга по шаблону или парсинга форм."
type: docs
weight: 860
url: /ru/net/groupdocs.parser.data/pagetextarea/
---

## PageTextArea class

Представляет текстовую область страницы, используемую для представления текстового значения в функции парсинга по шаблону или парсинга форм.

```csharp
public sealed class PageTextArea : PageArea
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | Инициализирует новый экземпляр класса [`PageTextArea`](../pagetextarea). |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | Инициализирует новый экземпляр класса [`PageTextArea`](../pagetextarea). |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | Инициализирует новый экземпляр класса [`PageTextArea`](../pagetextarea). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | Получает коллекцию дочерних текстовых областей страницы. |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | Получает базовую линию. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Возвращает информацию о странице документа, такую как индекс страницы и её размер. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Получает прямоугольную область. |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | Получает текст. |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | Получает стиль текста, такой как размер шрифта, название шрифта и т.д. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | Преобразует значение этого экземпляра в String. |

### Примечания

Экземпляр класса [`PageTextArea`](../pagetextarea) используется в качестве возвращаемого значения следующих методов:

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

Также экземпляр класса [`PageTextArea`](../pagetextarea) используется в качестве значения свойства [`PageArea`](../fielddata/pagearea).

Смотрите примеры использования там.

Текстовая область может быть одиночной или составной. В первом случае она содержит текст, ограниченный прямоугольной областью. Во втором случае она содержит другие текстовые области; свойства текста и таблицы вычисляются на основе дочерних текстовых областей.

### См. также

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
