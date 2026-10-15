---
title: "GetMetadata"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает метаданные из документа."
type: docs
weight: 140
url: /ru/net/groupdocs.parser/parser/getmetadata/
---

## Parser.GetMetadata method

Извлекает метаданные из документа.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### Возвращаемое значение

Коллекция элементов метаданных; `null`, если извлечение метаданных не поддерживается.

### Примечания

**Learn more:**

* [Extract metadata from documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Примеры

Следующий пример показывает, как извлечь метаданные из документа:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь метаданные из документа
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // Проверьте, поддерживается ли извлечение метаданных
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // Итерировать элементы метаданных
    foreach(MetadataItem item in metadata)
    {
        // Вывести имя элемента и его значение
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### См. также

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
