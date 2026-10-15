---
title: "IDocumentInfo"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет информацию о документе."
type: docs
weight: 370
url: /ru/net/groupdocs.parser.options/idocumentinfo/
---

## IDocumentInfo interface

Представляет информацию о документе.

```csharp
public interface IDocumentInfo
```

## Свойства

| Имя | Описание |
| --- | --- |
| [FileType](../../groupdocs.parser.options/idocumentinfo/filetype) { get; } | Возвращает тип документа. |
| [PageCount](../../groupdocs.parser.options/idocumentinfo/pagecount) { get; } | Получает общее количество страниц документа. |
| [Pages](../../groupdocs.parser.options/idocumentinfo/pages) { get; } | Получает информацию о страницах, такую как индекс и размер страницы. |
| [RawPageCount](../../groupdocs.parser.options/idocumentinfo/rawpagecount) { get; } | Получает общее количество необработанных страниц документа. |
| [Size](../../groupdocs.parser.options/idocumentinfo/size) { get; } | Возвращает размер документа в байтах. |

### Примечания

Объекты, реализующие этот интерфейс, возвращаются методом [`GetDocumentInfo`](../../groupdocs.parser/parser/getdocumentinfo). См. примеры использования там. **Узнать больше:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
