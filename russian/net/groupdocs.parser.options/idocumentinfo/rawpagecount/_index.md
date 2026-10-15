---
title: "RawPageCount"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Получает общее количество необработанных страниц документа."
type: docs
weight: 40
url: /ru/net/groupdocs.parser.options/idocumentinfo/rawpagecount/
---

## IDocumentInfo.RawPageCount property

Получает общее количество необработанных страниц документа.

```csharp
public int RawPageCount { get; }
```

### Property Value

Целочисленное значение, представляющее общее количество необработанных страниц.

### Примечания

Используйте свойство `RawPageCount` вместо свойства [`PageCount`](../pagecount) для извлечения необработанного текста. Некоторые документы имеют разные номера страниц в режимах точного и необработанного извлечения текста. Свойство [`PageCount`](../pagecount) может выполнять дополнительные вычисления, что влияет на скорость извлечения текста в необработанном режиме.

### См. также

* interface [IDocumentInfo](../../idocumentinfo)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
