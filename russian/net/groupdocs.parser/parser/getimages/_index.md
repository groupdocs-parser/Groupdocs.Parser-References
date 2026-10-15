---
title: "GetImages"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает изображения из документа."
type: docs
weight: 130
url: /ru/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

Извлекает изображения из документа.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Возвращаемое значение

Коллекция объектов [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null`, если извлечение изображений не поддерживается.

### Примечания

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Примеры

В следующем примере показано, как извлечь все изображения из всего документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь изображения
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Проверить, поддерживается ли извлечение изображений
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Перебрать изображения
    foreach (PageImageArea image in images)
    {
        // Вывести индекс страницы, прямоугольник и тип изображения:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### См. также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Извлекает изображения из документа с использованием параметров настройки (для задания прямоугольной области, содержащей изображения).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageAreaOptions | Параметры извлечения изображений. |

### Возвращаемое значение

Коллекция объектов [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null`, если извлечение изображений не поддерживается.

### Примечания

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Примеры

В следующем примере показано, как извлечь только изображения из верхнего левого угла:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Создайте параметры, которые используются для извлечения изображений
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Извлечь изображения из верхнего левого угла страницы:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Проверить, поддерживается ли извлечение изображений
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Перебрать изображения
    foreach (PageImageArea image in images)
    {
        // Вывести индекс страницы, прямоугольник и тип изображения:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### См. также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Извлекает изображения со страницы документа.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Коллекция объектов [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null`, если извлечение изображений не поддерживается.

### Примечания

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Примеры

Для извлечения изображений со страницы документа используется следующий метод:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение изображений
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверьте, есть ли у документа страницы
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Перебрать страницы
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Перебрать изображения
        // Мы игнорируем проверку на null, так как ранее проверили поддержку функции извлечения изображений
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Вывести прямоугольник и тип изображения
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### См. также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Извлекает изображения со страницы документа с использованием параметров настройки (для задания прямоугольной области, содержащей изображения).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | PageAreaOptions | Параметры извлечения изображений. |

### Возвращаемое значение

Коллекция объектов [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea); `null`, если извлечение изображений не поддерживается.

### Примечания

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### См. также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
