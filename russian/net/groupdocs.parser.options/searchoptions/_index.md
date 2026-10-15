---
title: "SearchOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, используемые для поиска текста."
type: docs
weight: 590
url: /ru/net/groupdocs.parser.options/searchoptions/
---

## SearchOptions class

Предоставляет параметры, используемые для поиска текста.

```csharp
public sealed class SearchOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions) с значениями по умолчанию. См. замечания для подробностей. |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions), который используется для поиска без извлечения подсветки. |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions), который используется для поиска по страницам и без извлечения подсветки. |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions), который используется для поиска с одинаковыми параметрами подсветки для левой и правой подсветки. |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions), который используется для поиска с параметрами подсветки для левой и правой подсветки. |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions). |
| [SearchOptions](searchoptions#constructor_6)(bool, bool, bool, int, HighlightOptions, HighlightOptions) | Инициализирует новый экземпляр класса [`SearchOptions`](../searchoptions) с ограничением по страницам. |

## Свойства

| Имя | Описание |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; set; } | Получает параметры для левой подсветки. |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; set; } | Возвращает значение, указывающее, не игнорируется ли регистр текста. |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; set; } | Получает значение, указывающее, ограничен ли поиск текста целым словом. |
| [MaxPageIndex](../../groupdocs.parser.options/searchoptions/maxpageindex) { get; set; } | Получает значение, представляющее максимальный индекс страницы для поиска. |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; set; } | Получает параметры для правой подсветки. |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; set; } | Получает значение, указывающее, выполняется ли поиск по страницам. |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; set; } | Получает значение, указывающее, используется ли регулярное выражение. |

### Примечания

Экземпляр класса [`SearchOptions`](../searchoptions) используется в качестве параметра метода [`Search`](../../groupdocs.parser/parser/search). См. примеры использования там.

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
