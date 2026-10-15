---
title: "GetImageStream"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Возвращает поток изображения."
type: docs
weight: 40
url: /ru/net/groupdocs.parser.data/pageimagearea/getimagestream/
---

## GetImageStream() {#getimagestream}

Возвращает поток изображения.

```csharp
public Stream GetImageStream()
```

### Возвращаемое значение

Поток с изображением.

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
        // Откройте поток изображения
        using (Stream imageStream = image.GetImageStream())
        {
            // Создайте файл для сохранения изображения
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Прочитайте данные из потока изображения
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Запишите данные в поток файла
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### См. также

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

Возвращает поток изображения в другом формате.

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | ImageOptions | Параметры, используемые для извлечения изображения. |

### Возвращаемое значение

Поток с изображением.

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
        // Откройте поток изображения
        using (Stream imageStream = image.GetImageStream(options))
        {
            // Создайте файл для сохранения изображения
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // Прочитайте данные из потока изображения
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // Запишите данные в поток файла
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### См. также

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
