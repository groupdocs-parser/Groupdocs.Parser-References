---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет область страницы, используемую для представления гиперссылки на странице."
type: docs
weight: 820
url: /ru/net/groupdocs.parser.data/pagehyperlinkarea/
---

## PageHyperlinkArea class

Представляет область страницы, используемую для представления гиперссылки на странице.

```csharp
public sealed class PageHyperlinkArea : PageArea
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageHyperlinkArea](pagehyperlinkarea)(string, string, Page, Rectangle) | Инициализирует новый экземпляр класса [`PageHyperlinkArea`](../pagehyperlinkarea). |

## Свойства

| Имя | Описание |
| --- | --- |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Возвращает информацию о странице документа, такую как индекс страницы и её размер. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Получает прямоугольную область. |
| [Text](../../groupdocs.parser.data/pagehyperlinkarea/text) { get; } | Получает текст гиперссылки. |
| [Url](../../groupdocs.parser.data/pagehyperlinkarea/url) { get; } | Получает URL гиперссылки. |

### Примечания

Экземпляр класса [`PageHyperlinkArea`](../pagehyperlinkarea) используется в качестве возвращаемого значения следующих методов:

* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)
* [`GetHyperlinks`](../../groupdocs.parser/parser/gethyperlinks)

Смотрите примеры использования там.

### См. также

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
