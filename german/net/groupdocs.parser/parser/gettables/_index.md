---
title: GetTables
second_title: GroupDocs.Parser für .NET-API-Referenz
description: Extrahiert Tabellen aus dem Dokument.
type: docs
weight: 140
url: /de/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Extrahiert Tabellen aus dem Dokument.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageTableAreaOptions | Die Optionen zum Extrahieren von Tabellen. |

### Rückgabewert

Eine Sammlung von[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) Objekte; `Null` wenn die Tabellenextraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Tabellen aus dem gesamten Dokument extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument Tabellenextraktion unterstützt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Tabellenlayout erstellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Erstellen Sie die Optionen für die Tabellenextraktion
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Tabellen aus dem Dokument extrahieren
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Über Tabellen iterieren
    foreach (PageTableArea t in tables)
    {
        // Über Zeilen iterieren
        for (int row = 0; row < t.RowCount; row++)
        {
            // Über Spalten iterieren
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Hole die Tabellenzelle
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Text der Tabellenzelle drucken
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

### Siehe auch

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Extrahiert Tabellen von der Dokumentseite.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageTableAreaOptions | Die Optionen zum Extrahieren von Tabellen. |

### Rückgabewert

Eine Sammlung von[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) Objekte; `Null` wenn die Tabellenextraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie Tabellen aus der Dokumentseite extrahiert werden:

```csharp
// Erstellen Sie eine Instanz der Parser-Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument Tabellenextraktion unterstützt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Tabellenlayout erstellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Erstellen Sie die Optionen für die Tabellenextraktion
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Holen Sie sich die Dokumentinformationen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Über Seiten iterieren
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Eine Seitenzahl drucken 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Tabellen aus der Dokumentseite extrahieren
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Über Tabellen iterieren
        foreach (PageTableArea t in tables)
        {
            // Über Zeilen iterieren
            for (int row = 0; row < t.RowCount; row++)
            {
                // Über Spalten iterieren
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Hole die Tabellenzelle
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Text der Tabellenzelle drucken
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

### Siehe auch

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namensraum [GroupDocs.Parser](../../parser)
* Montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
