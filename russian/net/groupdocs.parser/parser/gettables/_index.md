---
title: "GetTables"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает таблицы из документа."
type: docs
weight: 170
url: /ru/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Извлекает таблицы из документа.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageTableAreaOptions | Параметры извлечения таблиц. |

### Возвращаемое значение

Коллекция объектов [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null`, если извлечение таблиц не поддерживается.

### Примеры

В следующем примере показано, как извлечь таблицы из всего документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение таблиц
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Создайте макет таблиц
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Создайте параметры для извлечения таблиц
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Извлеките таблицы из документа
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Перебрать таблицы
    foreach (PageTableArea t in tables)
    {
        // Итерировать строки
        for (int row = 0; row < t.RowCount; row++)
        {
            // Итерировать столбцы
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Получить ячейку таблицы
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Вывести текст ячейки таблицы
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Извлекает таблицы со страницы документа.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | PageTableAreaOptions | Параметры извлечения таблиц. |

### Возвращаемое значение

Коллекция объектов [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null`, если извлечение таблиц не поддерживается.

### Примеры

В следующем примере показано, как извлечь таблицы со страницы документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение таблиц
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Создайте макет таблиц
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Создайте параметры для извлечения таблиц
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверьте, есть ли у документа страницы
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Перебрать страницы
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Извлечь таблицы со страницы документа
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Перебрать таблицы
        foreach (PageTableArea t in tables)
        {
            // Итерировать строки
            for (int row = 0; row < t.RowCount; row++)
            {
                // Итерировать столбцы
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Получить ячейку таблицы
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Вывести текст ячейки таблицы
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Извлекает таблицы из документа.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Возвращаемое значение

Коллекция объектов [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null`, если извлечение таблиц не поддерживается.

### Примеры

В следующем примере показано, как извлечь таблицы из всего документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение таблиц
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Извлеките таблицы из документа
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Перебрать таблицы
    foreach (PageTableArea t in tables)
    {
        // Итерировать строки
        for (int row = 0; row < t.RowCount; row++)
        {
            // Итерировать столбцы
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Получить ячейку таблицы
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Вывести текст ячейки таблицы
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Извлекает таблицы со страницы документа.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Коллекция объектов [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null`, если извлечение таблиц не поддерживается.

### Примеры

В следующем примере показано, как извлечь таблицы со страницы документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение таблиц
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверьте, есть ли у документа страницы
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Перебрать страницы
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Извлечь таблицы со страницы документа
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Перебрать таблицы
        foreach (PageTableArea t in tables)
        {
            // Итерировать строки
            for (int row = 0; row < t.RowCount; row++)
            {
                // Итерировать столбцы
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Получить ячейку таблицы
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Вывести текст ячейки таблицы
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
