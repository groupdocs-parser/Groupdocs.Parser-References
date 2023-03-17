---
title: GetTables
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Εξάγει πίνακες από το έγγραφο.
type: docs
weight: 140
url: /el/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Εξάγει πίνακες από το έγγραφο.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PageTableAreaOptions | Οι επιλογές για την εξαγωγή πινάκων. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) αντικείμενα; `μηδενικό` εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε πίνακες από ολόκληρο το έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή πίνακα
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Δημιουργία της διάταξης των πινάκων
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Δημιουργήστε τις επιλογές για εξαγωγή πίνακα
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Εξαγωγή πινάκων από το έγγραφο
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Επανάληψη πάνω από πίνακες
    foreach (PageTableArea t in tables)
    {
        // Επανάληψη σε γραμμές
        for (int row = 0; row < t.RowCount; row++)
        {
            // Επανάληψη σε στήλες
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Λήψη του κελιού του πίνακα
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Εκτυπώστε το κείμενο του κελιού του πίνακα
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

### Δείτε επίσης

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Εξάγει πίνακες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |
| options | PageTableAreaOptions | Οι επιλογές για την εξαγωγή πινάκων. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) αντικείμενα; `μηδενικό` εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε πίνακες από τη σελίδα του εγγράφου:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή πίνακα
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Δημιουργία της διάταξης των πινάκων
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Δημιουργήστε τις επιλογές για εξαγωγή πίνακα
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Λάβετε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε εάν το έγγραφο έχει σελίδες
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Επανάληψη σε σελίδες
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Εκτύπωση αριθμού σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Εξαγωγή πινάκων από τη σελίδα του εγγράφου
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Επανάληψη πάνω από πίνακες
        foreach (PageTableArea t in tables)
        {
            // Επανάληψη σε γραμμές
            for (int row = 0; row < t.RowCount; row++)
            {
                // Επανάληψη σε στήλες
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Λήψη του κελιού του πίνακα
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Εκτυπώστε το κείμενο του κελιού του πίνακα
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

### Δείτε επίσης

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
