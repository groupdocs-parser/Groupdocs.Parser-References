---
title: "GetTextAreas"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает области текста из документа."
type: docs
weight: 190
url: /ru/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

Извлекает области текста из документа.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Возвращаемое значение

Коллекция объектов [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null`, если извлечение областей текста не поддерживается.

### Примечания

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Примеры

В следующем примере показано, как извлечь все области текста из всего документа:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь области текста
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Проверьте, поддерживается ли извлечение областей текста
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Перебрать области текста страницы
    foreach(PageTextArea a in areas)
    {
        // Вывести индекс страницы, прямоугольник и значение области текста:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Извлекает области текста из документа, используя параметры настройки (регулярные выражения, учет регистра и т.д.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageTextAreaOptions | Параметры извлечения областей текста. |

### Возвращаемое значение

Коллекция объектов [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null`, если извлечение областей текста не поддерживается.

### Примечания

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Примеры

В следующем примере показано, как извлечь только области текста с цифрами из верхнего левого угла:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Создайте параметры, которые используются для извлечения областей текста
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Извлечь области текста, содержащие только цифры, из верхнего левого угла страницы:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Проверьте, поддерживается ли извлечение областей текста
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Перебрать области текста страницы
    foreach(PageTextArea a in areas)
    {
        // Вывести индекс страницы, прямоугольник и значение области текста:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Извлекает области текста со страницы документа.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Коллекция объектов [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null`, если извлечение областей текста не поддерживается.

### Примечания

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Примеры

Для извлечения областей текста со страницы документа используется следующий метод:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение областей текста
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверьте, есть ли у документа страницы
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Перебрать страницы
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Перебрать области текста страницы
        // Мы игнорируем проверку на null, так как ранее проверили поддержку функции извлечения областей текста
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Вывести прямоугольник и значение области текста:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Извлекает области текста со страницы документа, используя параметры настройки (регулярные выражения, учет регистра и т.д.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | PageTextAreaOptions | Параметры извлечения областей текста. |

### Возвращаемое значение

Коллекция объектов [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null`, если извлечение областей текста не поддерживается.

### Примечания

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
