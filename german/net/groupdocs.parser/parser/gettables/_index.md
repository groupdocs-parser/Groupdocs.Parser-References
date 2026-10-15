---
title: "GetTables"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Extrahiert Tabellen aus dem Dokument."
type: docs
weight: 170
url: /de/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Extrahiert Tabellen aus dem Dokument.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | PageTableAreaOptions | Die Optionen für die Tabellenextraktion. |

### Rückgabewert

Eine Sammlung von [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)-Objekten; `null`, wenn die Tabellenextraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Tabellen aus dem gesamten Dokument extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument die Tabellenextraktion unterstützt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Erstelle das Layout der Tabellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Erstelle die Optionen für die Tabellenextraktion
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Extrahiere Tabellen aus dem Dokument
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Iteriere über Tabellen
    foreach (PageTableArea t in tables)
    {
        // Iteriere über Zeilen
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iteriere über Spalten
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Hole die Tabellenzelle
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Gib den Text der Tabellenzelle aus
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Extrahiert Tabellen aus der Dokumentseite.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |
| options | PageTableAreaOptions | Die Optionen für die Tabellenextraktion. |

### Rückgabewert

Eine Sammlung von [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)-Objekten; `null`, wenn die Tabellenextraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Tabellen aus der Dokumentenseite extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument die Tabellenextraktion unterstützt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Erstelle das Layout der Tabellen
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Erstelle die Optionen für die Tabellenextraktion
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Rufe die Dokumentinformationen ab
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Iteriere über die Seiten
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extrahiere Tabellen aus der Dokumentenseite
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Iteriere über Tabellen
        foreach (PageTableArea t in tables)
        {
            // Iteriere über Zeilen
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iteriere über Spalten
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Hole die Tabellenzelle
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Gib den Text der Tabellenzelle aus
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Extrahiert Tabellen aus dem Dokument.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Rückgabewert

Eine Sammlung von [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)-Objekten; `null`, wenn die Tabellenextraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Tabellen aus dem gesamten Dokument extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument die Tabellenextraktion unterstützt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Extrahiere Tabellen aus dem Dokument
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Iteriere über Tabellen
    foreach (PageTableArea t in tables)
    {
        // Iteriere über Zeilen
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iteriere über Spalten
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Hole die Tabellenzelle
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Gib den Text der Tabellenzelle aus
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
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Extrahiert Tabellen aus der Dokumentseite.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | Int32 | Der nullbasierte Seitenindex. |

### Rückgabewert

Eine Sammlung von [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea)-Objekten; `null`, wenn die Tabellenextraktion nicht unterstützt wird.

### Beispiele

Das folgende Beispiel zeigt, wie man Tabellen aus der Dokumentenseite extrahiert:

```csharp
// Erstelle eine Instanz der Parser‑Klasse
using (Parser parser = new Parser(filePath))
{
    // Prüfen, ob das Dokument die Tabellenextraktion unterstützt
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Rufe die Dokumentinformationen ab
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Prüfe, ob das Dokument Seiten hat
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Iteriere über die Seiten
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Gib eine Seitenzahl aus 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Extrahiere Tabellen aus der Dokumentenseite
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Iteriere über Tabellen
        foreach (PageTableArea t in tables)
        {
            // Iteriere über Zeilen
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iteriere über Spalten
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Hole die Tabellenzelle
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Gib den Text der Tabellenzelle aus
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
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
