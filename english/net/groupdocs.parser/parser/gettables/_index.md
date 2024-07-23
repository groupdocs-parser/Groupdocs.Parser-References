---
title: GetTables
second_title: GroupDocs.Parser for .NET API Reference
description: Extracts tables from the document.
type: docs
weight: 150
url: /net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Extracts tables from the document.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | PageTableAreaOptions | The options for tables extraction. |

### Return Value

A collection of [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objects; `null` if tables extraction isn't supported.

### Examples

The following example shows how to extract tables from the whole document:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Check if the document supports table extraction
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Create the layout of tables
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Create the options for table extraction
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extract tables from the document
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Iterate over tables
    foreach (PageTableArea t in tables)
    {
        // Iterate over rows
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iterate over columns
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Get the table cell
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Print the table cell text
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

### See Also

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Extracts tables from the document page.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The zero-based page index. |
| options | PageTableAreaOptions | The options for tables extraction. |

### Return Value

A collection of [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objects; `null` if tables extraction isn't supported.

### Examples

The following example shows how to extract tables from the document page:

```csharp
// Create an instance of Parser class
using (Parser parser = new Parser(filePath))
{
    // Check if the document supports table extraction
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Create the layout of tables
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Create the options for table extraction
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Get the document info
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Check if the document has pages
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iterate over pages
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print a page number 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extract tables from the document page
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Iterate over tables
        foreach (PageTableArea t in tables)
        {
            // Iterate over rows
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iterate over columns
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Get the table cell
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Print the table cell text
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

### See Also

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
