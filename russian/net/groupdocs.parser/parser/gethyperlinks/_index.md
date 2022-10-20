---
title: GetHyperlinks
second_title: Справочник по API GroupDocs.Parser для .NET
description: Извлекает гиперссылки из документа.
type: docs
weight: 100
url: /ru/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Извлекает гиперссылки из документа.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Возвращаемое значение

Коллекция[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) объекты; `нулевой` если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь все гиперссылки из всего документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Извлекаем гиперссылки из документа
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Перебираем гиперссылки
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Печатаем текст гиперссылки
        Console.WriteLine(h.Text);
        // Печатаем URL-адрес гиперссылки
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Смотрите также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Извлекает гиперссылки со страницы документа.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |

### Возвращаемое значение

Коллекция[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) объекты; `нулевой` если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь гиперссылки со страницы документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Печатаем номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Извлекаем гиперссылки со страницы документа
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Перебираем гиперссылки
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Печатаем текст гиперссылки
            Console.WriteLine(h.Text);
            // Печатаем URL-адрес гиперссылки
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Смотрите также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Извлекает гиперссылки из документа с помощью параметров настройки (для установки прямоугольной области, содержащей гиперссылки).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageAreaOptions | Варианты извлечения гиперссылок. |

### Возвращаемое значение

Коллекция[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) объекты; `нулевой` если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь гиперссылки из области страницы документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Создаем параметры, которые используются для извлечения гиперссылок
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Извлечение гиперссылок из области страницы документа
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Перебираем гиперссылки
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Печатаем текст гиперссылки
        Console.WriteLine(h.Text);
        // Печатаем URL-адрес гиперссылки
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Смотрите также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Извлекает гиперссылки со страницы документа с помощью параметров настройки (для установки прямоугольной области, содержащей гиперссылки).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |
| options | PageAreaOptions | Варианты извлечения гиперссылок. |

### Возвращаемое значение

Коллекция[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) объекты; `нулевой` если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь гиперссылки из области страницы документа с помощью параметров настройки:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    
    // Создаем параметры, которые используются для извлечения гиперссылок
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Перебираем страницы
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Печатаем номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Извлечение гиперссылок из области страницы документа
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Перебираем гиперссылки
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Печатаем текст гиперссылки
            Console.WriteLine(h.Text);
            // Печатаем URL-адрес гиперссылки
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Смотрите также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
