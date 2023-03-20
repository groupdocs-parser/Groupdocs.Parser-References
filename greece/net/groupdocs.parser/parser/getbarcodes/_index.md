---
title: GetBarcodes
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Εξάγει γραμμικούς κώδικες από το έγγραφο.
type: docs
weight: 50
url: /el/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Εξάγει γραμμικούς κώδικες από το έγγραφο.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) αντικείμενα; `μηδενικό` αν δεν υποστηρίζεται η εξαγωγή γραμμωτών κωδίκων.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε γραμμικούς κώδικες από ένα έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Εξαγωγή γραμμωτών κωδίκων από το έγγραφο.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Επανάληψη σε γραμμωτούς κώδικες
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Εκτύπωση του ευρετηρίου σελίδας
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Εκτυπώστε την τιμή του γραμμικού κώδικα
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) αντικείμενα; `μηδενικό` αν δεν υποστηρίζεται η εξαγωγή γραμμωτών κωδίκων.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε γραμμικούς κώδικες από μια σελίδα εγγράφου:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Εξαγωγή γραμμωτών κωδίκων από τη δεύτερη σελίδα εγγράφου.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Επανάληψη σε γραμμωτούς κώδικες
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Εκτύπωση του ευρετηρίου σελίδας
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Εκτυπώστε την τιμή του γραμμικού κώδικα
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Εξάγει γραμμικούς κώδικες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει γραμμικούς κώδικες).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή barcodes. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) αντικείμενα; `μηδενικό` αν δεν υποστηρίζεται η εξαγωγή γραμμωτών κωδίκων.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε γραμμικούς κώδικες από την επάνω δεξιά γωνία.

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή γραμμωτών κωδίκων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Εξαγωγή γραμμωτών κωδίκων από την επάνω δεξιά γωνία.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Επανάληψη σε γραμμωτούς κώδικες
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Εκτύπωση του ευρετηρίου σελίδας
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Εκτυπώστε την τιμή του γραμμικού κώδικα
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει γραμμικούς κώδικες).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή barcodes. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) αντικείμενα; `μηδενικό` αν δεν υποστηρίζεται η εξαγωγή γραμμωτών κωδίκων.

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
