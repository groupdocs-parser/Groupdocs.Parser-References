---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает гиперссылки из документа."
type: docs
weight: 120
url: /ru/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

Извлекает гиперссылки из документа.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Возвращаемое значение

Коллекция объектов [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null`, если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь все гиперссылки из всего документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Извлечь гиперссылки из документа
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Перебрать гиперссылки
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Вывести текст гиперссылки
        Console.WriteLine(h.Text);
        // Вывести URL гиперссылки
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### См. также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Извлекает гиперссылки со страницы документа.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Коллекция объектов [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null`, если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь гиперссылки со страницы документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Извлечь гиперссылки со страницы документа
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Перебрать гиперссылки
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Вывести текст гиперссылки
            Console.WriteLine(h.Text);
            // Вывести URL гиперссылки
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### См. также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Извлекает гиперссылки из документа с использованием параметров настройки (для задания прямоугольной области, содержащей гиперссылки).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageAreaOptions | Параметры извлечения гиперссылок. |

### Возвращаемое значение

Коллекция объектов [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null`, если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлечь гиперссылки из области страницы документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Создать параметры, используемые для извлечения гиперссылок
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Извлечь гиперссылки из области страницы документа
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Перебрать гиперссылки
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Вывести текст гиперссылки
        Console.WriteLine(h.Text);
        // Вывести URL гиперссылки
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### См. также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Извлекает гиперссылки со страницы документа с использованием параметров настройки (для задания прямоугольной области, содержащей гиперссылки).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | PageAreaOptions | Параметры извлечения гиперссылок. |

### Возвращаемое значение

Коллекция объектов [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null`, если извлечение гиперссылок не поддерживается.

### Примеры

В следующем примере показано, как извлекать гиперссылки из области страницы документа, используя параметры настройки:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение гиперссылок
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    
    // Создать параметры, используемые для извлечения гиперссылок
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Перебрать страницы
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Извлечь гиперссылки из области страницы документа
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Перебрать гиперссылки
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Вывести текст гиперссылки
            Console.WriteLine(h.Text);
            // Вывести URL гиперссылки
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### См. также

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
