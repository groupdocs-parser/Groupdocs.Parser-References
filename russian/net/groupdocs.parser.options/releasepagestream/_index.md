---
title: "ReleasePageStream"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет метод, который освобождает поток, созданный делегатом CreatePageStream./createpagestream."
type: docs
weight: 580
url: /ru/net/groupdocs.parser.options/releasepagestream/
---

## ReleasePageStream delegate

Представляет метод, который освобождает поток, созданный делегатом [`CreatePageStream`](../createpagestream).

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageNumber | Int32 | Номер страницы сгенерированного предварительного просмотра. |
| pageStream | Stream | Поток, содержащий сгенерированный предварительный просмотр страницы. |

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
