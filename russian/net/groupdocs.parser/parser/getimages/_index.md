---
title: GetImages
second_title: Справочник по API GroupDocs.Parser для .NET
description: Извлекает изображения из документа.
type: docs
weight: 110
url: /ru/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Извлекает изображения из документа.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Возвращаемое значение

Коллекция[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) объекты; `нулевой` если извлечение изображений не поддерживается.

### Примечания

**Учить больше:**

* [Извлечение изображений из документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Извлечь изображения в файлы](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Извлечение изображений из документов Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Извлечение изображений из электронных таблиц Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Извлечение изображений из презентаций Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Извлечение изображений из электронных писем](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Извлечение изображений из PDF-документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Примеры

В следующем примере показано, как извлечь все изображения из всего документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечение изображений
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Проверяем, поддерживается ли извлечение изображений
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Перебираем изображения
    foreach (PageImageArea image in images)
    {
        // Печатаем индекс страницы, прямоугольник и тип изображения:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Смотрите также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Извлекает изображения из документа с помощью параметров настройки (для установки прямоугольной области, содержащей изображения).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageAreaOptions | Варианты извлечения изображений. |

### Возвращаемое значение

Коллекция[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) объекты; `нулевой` если извлечение изображений не поддерживается.

### Примечания

**Учить больше:**

* [Извлечение изображений из документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Извлечь изображения в файлы](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Извлечение изображений из области страницы документа](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Извлечение изображений из документов Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Извлечение изображений из электронных таблиц Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Извлечение изображений из презентаций Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Извлечение изображений из электронных писем](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Извлечение изображений из PDF-документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Примеры

В следующем примере показано, как извлечь только изображения из верхнего левого угла:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Создаем параметры, которые используются для извлечения изображений
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Извлечь изображения из верхнего левого угла страницы:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Проверяем, поддерживается ли извлечение изображений
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Перебираем изображения
    foreach (PageImageArea image in images)
    {
        // Печатаем индекс страницы, прямоугольник и тип изображения:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Смотрите также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Извлекает изображения со страницы документа.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |

### Возвращаемое значение

Коллекция[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) объекты; `нулевой` если извлечение изображений не поддерживается.

### Примечания

**Учить больше:**

* [Извлечение изображений из документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Извлечь изображения в файлы](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Извлечь изображения со страницы документа](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Извлечение изображений из документов Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Извлечение изображений из электронных таблиц Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Извлечение изображений из презентаций Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Извлечение изображений из электронных писем](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Извлечение изображений из PDF-документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Примеры

Для извлечения изображений со страницы документа используется следующий метод:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение изображений
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверяем, есть ли в документе страницы
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Перебираем страницы
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Печатаем номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Перебираем изображения
        // Мы игнорируем проверку на null, так как мы проверили поддержку функции извлечения изображений ранее
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Печатаем прямоугольник и тип изображения
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Смотрите также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Извлекает изображения со страницы документа с помощью параметров настройки (для установки прямоугольной области, содержащей изображения).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |
| options | PageAreaOptions | Варианты извлечения изображений. |

### Возвращаемое значение

Коллекция[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) объекты; `нулевой` если извлечение изображений не поддерживается.

### Примечания

**Учить больше:**

* [Извлечение изображений из документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Извлечь изображения в файлы](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Извлечь изображения со страницы документа](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Извлечение изображений из области страницы документа](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Извлечение изображений из документов Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Извлечение изображений из электронных таблиц Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Извлечение изображений из презентаций Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Извлечение изображений из электронных писем](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Извлечение изображений из PDF-документов](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Смотрите также

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
