---
title: "DetectFileType"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Определяет тип файла элемента контейнера."
type: docs
weight: 60
url: /ru/net/groupdocs.parser.data/containeritem/detectfiletype/
---

## ContainerItem.DetectFileType method

Определяет тип файла элемента контейнера.

```csharp
public FileType DetectFileType(FileTypeDetectionMode detectionMode)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| detectionMode | FileTypeDetectionMode | Определяет режим обнаружения типа файла. |

### Возвращаемое значение

Экземпляр класса [`FileType`](../../../groupdocs.parser.options/filetype); [`Unknown`](../../../groupdocs.parser.options/filetype/unknown), если тип файла не обнаружен.

### Примечания

*detectionMode* parameter provides the ability to control file type detection:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

### Примеры

Следующий пример показывает, как определить тип файла элемента контейнера:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь вложения из контейнера
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // Проверьте, поддерживается ли извлечение контейнера
    if (attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
    // Переберите вложения
    foreach (ContainerItem item in attachments)
    {
        // Определите тип файла
        Options.FileType fileType = item.DetectFileType(Options.FileTypeDetectionMode.Default);

        // Выведите имя и тип файла
        Console.WriteLine(string.Format("{0}: {1}", item.Name, fileType));
    }
}
```

### См. также

* class [FileType](../../../groupdocs.parser.options/filetype)
* enum [FileTypeDetectionMode](../../../groupdocs.parser.options/filetypedetectionmode)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
