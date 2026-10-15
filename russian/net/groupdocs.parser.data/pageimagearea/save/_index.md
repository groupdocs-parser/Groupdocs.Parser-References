---
title: "Сохранить"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Сохраняет изображение в файл."
type: docs
weight: 50
url: /ru/net/groupdocs.parser.data/pageimagearea/save/
---

## Save(string) {#save}

Сохраняет изображение в файл.

```csharp
public void Save(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |

### Примеры

В следующем примере показано, как сохранять изображения в файлы:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь изображения из документа
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Проверить, поддерживается ли извлечение изображений
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Перебрать изображения
    foreach (PageImageArea image in images)
    {
        // Сохраните изображение в файл
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### См. также

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

Сохраняет изображение в файл в другом формате.

```csharp
public void Save(string filePath, ImageOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |
| options | ImageOptions | Параметры, используемые для сохранения изображения. |

### Примеры

Следующий пример показывает, как сохранять изображения в файлы в другом формате:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь изображения из документа
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // Проверить, поддерживается ли извлечение изображений
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // Создайте параметры для сохранения изображений в формате PNG
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // Перебрать изображения
    foreach (PageImageArea image in images)
    {
        // Сохраните изображение в файл PNG
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### См. также

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
