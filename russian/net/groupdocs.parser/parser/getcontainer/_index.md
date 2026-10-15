---
title: "GetContainer"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает объект контейнера из документа для работы с форматами, содержащими вложения, ZIP‑архивы и т.п."
type: docs
weight: 80
url: /ru/net/groupdocs.parser/parser/getcontainer/
---

## Parser.GetContainer method

Извлекает объект‑контейнер из документа для работы с форматами, содержащими вложения, ZIP‑архивы и т.п.

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### Возвращаемое значение

Коллекция элементов контейнера; `null`, если извлечение контейнера не поддерживается.

### Примечания

Чтобы проверить, поддерживает ли формат извлечение вложений, см. [Supported Document Formats](https://docs.groupdocs.com/parser/net/supported-document-formats/) (столбец **Extract Containers and Attachments**).

**Learn more:**

* [Extract data from attachments and ZIP archives](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### Примеры

В следующем примере показано, как извлечь вложения из контейнера:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь вложения из контейнера
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Проверьте, поддерживается ли извлечение контейнера
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // Переберите вложения
    foreach(ContainerItem item in attachments)
    {
        // Выведите имя элемента и его размер
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### См. также

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
