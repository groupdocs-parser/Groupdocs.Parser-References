---
title: GetTextAreas
second_title: Справочник по API GroupDocs.Parser для .NET
description: Извлекает текстовые области из документа.
type: docs
weight: 160
url: /ru/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Извлекает текстовые области из документа.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Возвращаемое значение

Коллекция[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) объекты; `нулевой` если извлечение текстовых областей не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текстовые области](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Примеры

В следующем примере показано, как извлечь все текстовые области из всего документа:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечение текстовых областей
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Проверяем, поддерживается ли извлечение текстовых областей
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Итерация по текстовым областям страницы
    foreach(PageTextArea a in areas)
    {
        // Печать индекса страницы, прямоугольника и значения текстовой области:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Смотрите также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Извлекает текстовые области из документа, используя параметры настройки (регулярное выражение, регистр и т. д.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageTextAreaOptions | Варианты выделения текстовой области. |

### Возвращаемое значение

Коллекция[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) объекты; `нулевой` если извлечение текстовых областей не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текстовые области](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Примеры

В следующем примере показано, как извлечь только текстовые области с цифрами из верхнего левого угла:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Создаем параметры, которые используются для выделения текстовой области
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Извлечение текстовых областей, содержащих только цифры, из левого верхнего угла страницы:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Проверяем, поддерживается ли извлечение текстовых областей
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Итерация по текстовым областям страницы
    foreach(PageTextArea a in areas)
    {
        // Печать индекса страницы, прямоугольника и значения текстовой области:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Смотрите также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Извлекает текстовые области со страницы документа.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |

### Возвращаемое значение

Коллекция[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) объекты; `нулевой` если извлечение текстовых областей не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текстовые области](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Примеры

Для извлечения текстовых областей со страницы документа используется следующий метод:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение текстовых областей
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверяем, есть ли в документе страницы
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Перебираем страницы
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Печатаем номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Итерация по текстовым областям страницы
        // Мы игнорируем проверку на null, так как мы проверили поддержку функции извлечения текстовых областей ранее
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Печать прямоугольника и значения текстовой области:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Смотрите также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Извлекает текстовые области со страницы документа, используя параметры настройки (регулярное выражение, регистр и т. д.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |
| options | PageTextAreaOptions | Варианты выделения текстовой области. |

### Возвращаемое значение

Коллекция[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) объекты; `нулевой` если извлечение текстовых областей не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текстовые области](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Смотрите также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
