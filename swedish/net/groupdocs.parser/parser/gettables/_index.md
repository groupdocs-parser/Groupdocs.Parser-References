---
title: GetTables
second_title: GroupDocs.Parser för .NET API-referens
description: Extraherar tabeller från dokumentet.
type: docs
weight: 140
url: /sv/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Extraherar tabeller från dokumentet.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | PageTableAreaOptions | Alternativen för tabellextraktion. |

### Returvärde

En samling av[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objekt; `null` om tabellextraktion inte stöds.

### Exempel

Följande exempel visar hur man extraherar tabeller från hela dokumentet:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder tabellextraktion
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Skapa layouten för tabeller
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Skapa alternativen för tabellextraktion
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extrahera tabeller från dokumentet
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Iterera över tabeller
    foreach (PageTableArea t in tables)
    {
        // Iterera över rader
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iterera över kolumner
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Hämta tabellcellen
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Skriv ut tabellcelltexten
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

### Se även

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Extraherar tabeller från dokumentsidan.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Det nollbaserade sidindexet. |
| options | PageTableAreaOptions | Alternativen för tabellextraktion. |

### Returvärde

En samling av[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objekt; `null` om tabellextraktion inte stöds.

### Exempel

Följande exempel visar hur man extraherar tabeller från dokumentsidan:

```csharp
// Skapa en instans av Parser-klassen
using (Parser parser = new Parser(filePath))
{
    // Kontrollera om dokumentet stöder tabellextraktion
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Skapa layouten för tabeller
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Skapa alternativen för tabellextraktion
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Få dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Kontrollera om dokumentet har sidor
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iterera över sidor
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Skriv ut ett sidnummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extrahera tabeller från dokumentsidan
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Iterera över tabeller
        foreach (PageTableArea t in tables)
        {
            // Iterera över rader
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iterera över kolumner
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Hämta tabellcellen
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Skriv ut tabellcelltexten
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

### Se även

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namnutrymme [GroupDocs.Parser](../../parser)
* hopsättning [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
