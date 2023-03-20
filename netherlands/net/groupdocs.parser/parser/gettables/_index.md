---
title: GetTables
second_title: GroupDocs.Parser voor .NET API-referentie
description: Haalt tabellen uit het document.
type: docs
weight: 140
url: /nl/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Haalt tabellen uit het document.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageTableAreaOptions | De opties voor het extraheren van tabellen. |

### Winstwaarde

Een verzameling van[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objecten; `nul` als extractie van tabellen niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe tabellen uit het hele document kunnen worden geëxtraheerd:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document tabelextractie ondersteunt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Maak de lay-out van tabellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Maak de opties voor tabelextractie
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extraheer tabellen uit het document
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Itereren over tabellen
    foreach (PageTableArea t in tables)
    {
        // Itereren over rijen
        for (int row = 0; row < t.RowCount; row++)
        {
            // Itereren over kolommen
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Haal de tabelcel op
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Druk de tabelceltekst af
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

### Zie ook

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Haalt tabellen uit de documentpagina.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De op nul gebaseerde pagina-index. |
| options | PageTableAreaOptions | De opties voor het extraheren van tabellen. |

### Winstwaarde

Een verzameling van[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objecten; `nul` als extractie van tabellen niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u tabellen uit de documentpagina haalt:

```csharp
// Maak een instantie van de Parser-klasse
using (Parser parser = new Parser(filePath))
{
    // Controleer of het document tabelextractie ondersteunt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Maak de lay-out van tabellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Maak de opties voor tabelextractie
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Haal de documentinfo op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Herhaal pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Druk een paginanummer af 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extraheer tabellen van de documentpagina
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Itereren over tabellen
        foreach (PageTableArea t in tables)
        {
            // Itereren over rijen
            for (int row = 0; row < t.RowCount; row++)
            {
                // Itereren over kolommen
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Haal de tabelcel op
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Druk de tabelceltekst af
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

### Zie ook

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* naamruimte [GroupDocs.Parser](../../parser)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
