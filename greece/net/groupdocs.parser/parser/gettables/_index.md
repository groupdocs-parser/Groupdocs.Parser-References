---
title: "GetTables"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει πίνακες από το έγγραφο."
type: docs
weight: 170
url: /el/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Εξάγει πίνακες από το έγγραφο.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| options | PageTableAreaOptions | Οι επιλογές για την εξαγωγή πινάκων. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε πίνακες από ολόκληρο το έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή πινάκων
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Δημιουργήστε τη διάταξη των πινάκων
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Δημιουργήστε τις επιλογές για την εξαγωγή πινάκων
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Εξάγετε πίνακες από το έγγραφο
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Επανάληψη πάνω στους πίνακες
    foreach (PageTableArea t in tables)
    {
        // Επανάληψη πάνω στις γραμμές
        for (int row = 0; row < t.RowCount; row++)
        {
            // Επανάληψη πάνω στις στήλες
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Αποκτήστε το κελί του πίνακα
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Εξάγει πίνακες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |
| options | PageTableAreaOptions | Οι επιλογές για την εξαγωγή πινάκων. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε πίνακες από τη σελίδα του εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή πινάκων
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Δημιουργήστε τη διάταξη των πινάκων
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Δημιουργήστε τις επιλογές για την εξαγωγή πινάκων
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Αποκτήστε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε αν το έγγραφο έχει σελίδες
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Διατρέξτε τις σελίδες
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Εξάγετε πίνακες από τη σελίδα του εγγράφου
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Επανάληψη πάνω στους πίνακες
        foreach (PageTableArea t in tables)
        {
            // Επανάληψη πάνω στις γραμμές
            for (int row = 0; row < t.RowCount; row++)
            {
                // Επανάληψη πάνω στις στήλες
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Αποκτήστε το κελί του πίνακα
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
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Εξάγει πίνακες από το έγγραφο.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε πίνακες από ολόκληρο το έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή πινάκων
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Εξάγετε πίνακες από το έγγραφο
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Επανάληψη πάνω στους πίνακες
    foreach (PageTableArea t in tables)
    {
        // Επανάληψη πάνω στις γραμμές
        for (int row = 0; row < t.RowCount; row++)
        {
            // Επανάληψη πάνω στις στήλες
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Αποκτήστε το κελί του πίνακα
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
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Εξάγει πίνακες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε πίνακες από τη σελίδα του εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή πινάκων
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Αποκτήστε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε αν το έγγραφο έχει σελίδες
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Διατρέξτε τις σελίδες
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Εξάγετε πίνακες από τη σελίδα του εγγράφου
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Επανάληψη πάνω στους πίνακες
        foreach (PageTableArea t in tables)
        {
            // Επανάληψη πάνω στις γραμμές
            for (int row = 0; row < t.RowCount; row++)
            {
                // Επανάληψη πάνω στις στήλες
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Αποκτήστε το κελί του πίνακα
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
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
