---
title: "ExtractText"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает текст из документа, к которому относится объект TocItemgroupdocs.parser.data/tocitem."
type: docs
weight: 50
url: /ru/net/groupdocs.parser.data/tocitem/extracttext/
---

## TocItem.ExtractText method

Извлекает текст из документа, к которому относится объект [`TocItem`](../../tocitem).

```csharp
public virtual TextReader ExtractText()
```

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом.

### Примеры

Следующий пример показывает, как извлечь текст с помощью элемента оглавления:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(Constants.SampleDocxWithToc))
{
    // Получить оглавление
    IEnumerable<TocItem> tocItems = parser.GetToc();
    // Проверьте, поддерживается ли извлечение оглавления
    if (tocItems == null)
    {
        Console.WriteLine("Table of contents extraction isn't supported");
    }
    // Перебрать элементы
    foreach (TocItem tocItem in tocItems)
    {
        // Вывести текст главы
        using (TextReader reader = tocItem.ExtractText())
        {
            Console.WriteLine("----");
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [TocItem](../../tocitem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
