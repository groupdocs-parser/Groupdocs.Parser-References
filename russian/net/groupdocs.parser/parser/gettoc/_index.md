---
title: "GetToc"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает оглавление из документа."
type: docs
weight: 200
url: /ru/net/groupdocs.parser/parser/gettoc/
---

## Parser.GetToc method

Извлекает оглавление из документа.

```csharp
public IEnumerable<TocItem> GetToc()
```

### Возвращаемое значение

Коллекция элементов оглавления; `null`, если извлечение оглавления не поддерживается.

### Примечания

**Learn more:**

* [Extract table of contents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Extract text by table of contents item](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### Примеры

В следующем примере показано, как извлечь оглавление из CHM‑файла:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживается ли извлечение текста
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }

    // Проверьте, поддерживается ли извлечение оглавления
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
 
    // Получить оглавление
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // Перебрать элементы
    foreach (TocItem i in toc)
    {
        // Выведите текст оглавления
        Console.WriteLine(i.Text);
        // Проверьте, имеет ли индекс страницы значение
        if (i.PageIndex == null)
        {
            continue;
        }
        // Извлеките текст страницы
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
