---
title: "GetDocumentInfo"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Возвращает общую информацию о документе."
type: docs
weight: 90
url: /ru/net/groupdocs.parser/parser/getdocumentinfo/
---

## Parser.GetDocumentInfo method

Возвращает общую информацию о документе.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Возвращаемое значение

Экземпляр класса, реализующего интерфейс [`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo).

### Примечания

**Learn more:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Примеры

В следующем примере показано, как получить информацию о документе:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Получить информацию о документе
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### См. также

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
