---
title: GetTables
second_title: Справочник по API GroupDocs.Parser для .NET
description: Извлекает таблицы из документа.
type: docs
weight: 140
url: /ru/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Извлекает таблицы из документа.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageTableAreaOptions | Варианты извлечения таблиц. |

### Возвращаемое значение

Коллекция[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) объекты; `нулевой` если извлечение таблиц не поддерживается.

### Примеры

В следующем примере показано, как извлечь таблицы из всего документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение таблицы
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Создаем раскладку таблиц
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Создаем опции для извлечения таблицы
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Извлечь таблицы из документа
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Итерация по таблицам
    foreach (PageTableArea t in tables)
    {
        // Перебираем строки
        for (int row = 0; row < t.RowCount; row++)
        {
            // Итерация по столбцам
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Получаем ячейку таблицы
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Печатаем текст ячейки таблицы
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

### Смотрите также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Извлекает таблицы со страницы документа.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |
| options | PageTableAreaOptions | Варианты извлечения таблиц. |

### Возвращаемое значение

Коллекция[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) объекты; `нулевой` если извлечение таблиц не поддерживается.

### Примеры

В следующем примере показано, как извлечь таблицы из страницы документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение таблицы
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Создаем раскладку таблиц
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Создаем опции для извлечения таблицы
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
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
        // Извлечение таблиц со страницы документа
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Итерация по таблицам
        foreach (PageTableArea t in tables)
        {
            // Перебираем строки
            for (int row = 0; row < t.RowCount; row++)
            {
                // Итерация по столбцам
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Получаем ячейку таблицы
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Печатаем текст ячейки таблицы
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

### Смотрите также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
