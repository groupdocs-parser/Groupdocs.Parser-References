---
title: "GetTables"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Extraheert tabellen uit het document."
type: docs
weight: 170
url: /nl/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Extraheert tabellen uit het document.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | PageTableAreaOptions | De opties voor het extraheren van tabellen. |

### Retourwaarde

Een verzameling van [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objecten; `null` als het extraheren van tabellen niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe tabellen uit het volledige document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleren of het document tabelextractie ondersteunt
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
    // Tabellen uit het document extraheren
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Itereer over tabellen
    foreach (PageTableArea t in tables)
    {
        // Itereer over rijen
        for (int row = 0; row < t.RowCount; row++)
        {
            // Itereer over kolommen
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Haal de tabelcel op
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Print de tekst van de tabelcel
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Extraheert tabellen van de documentpagina.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |
| options | PageTableAreaOptions | De opties voor het extraheren van tabellen. |

### Retourwaarde

Een verzameling van [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objecten; `null` als het extraheren van tabellen niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe tabellen van de documentpagina te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleren of het document tabelextractie ondersteunt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Maak de lay-out van tabellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Maak de opties voor tabelextractie
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Haal de documentinformatie op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Itereer over pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Tabellen van de documentpagina extraheren
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Itereer over tabellen
        foreach (PageTableArea t in tables)
        {
            // Itereer over rijen
            for (int row = 0; row < t.RowCount; row++)
            {
                // Itereer over kolommen
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Haal de tabelcel op
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Print de tekst van de tabelcel
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Extraheert tabellen uit het document.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Retourwaarde

Een verzameling van [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objecten; `null` als het extraheren van tabellen niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe tabellen uit het volledige document te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleren of het document tabelextractie ondersteunt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Tabellen uit het document extraheren
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Itereer over tabellen
    foreach (PageTableArea t in tables)
    {
        // Itereer over rijen
        for (int row = 0; row < t.RowCount; row++)
        {
            // Itereer over kolommen
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Haal de tabelcel op
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Print de tekst van de tabelcel
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
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Extraheert tabellen van de documentpagina.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageIndex | Int32 | De nulgebaseerde paginapositie. |

### Retourwaarde

Een verzameling van [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objecten; `null` als het extraheren van tabellen niet wordt ondersteund.

### Voorbeelden

Het volgende voorbeeld toont hoe tabellen van de documentpagina te extraheren:

```csharp
// Maak een instantie van de Parser‑klasse
using (Parser parser = new Parser(filePath))
{
    // Controleren of het document tabelextractie ondersteunt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Haal de documentinformatie op
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Controleer of het document pagina's heeft
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Itereer over pagina's
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Print een paginanummer 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Tabellen van de documentpagina extraheren
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Itereer over tabellen
        foreach (PageTableArea t in tables)
        {
            // Itereer over rijen
            for (int row = 0; row < t.RowCount; row++)
            {
                // Itereer over kolommen
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Haal de tabelcel op
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Print de tekst van de tabelcel
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
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
