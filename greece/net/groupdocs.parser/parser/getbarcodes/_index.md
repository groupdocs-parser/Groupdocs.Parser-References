---
title: "GetBarcodes"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει γραμμικούς κώδικες από το έγγραφο."
type: docs
weight: 70
url: /el/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Εξάγει γραμμικούς κώδικες από το έγγραφο.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)· `null` εάν η εξαγωγή κωδικών barcodes δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε γραμμωτούς κώδικες από ένα έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Εξάγετε γραμμωτούς κώδικες από το έγγραφο.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Διατρέξτε τους γραμμωτούς κώδικες
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Εκτυπώστε τον δείκτη της σελίδας
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Εκτυπώστε την τιμή του γραμμωτού κώδικα
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)· `null` εάν η εξαγωγή κωδικών barcodes δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε γραμμωτούς κώδικες από μια σελίδα εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Εξάγετε γραμμωτούς κώδικες από τη δεύτερη σελίδα του εγγράφου.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Διατρέξτε τους γραμμωτούς κώδικες
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Εκτυπώστε τον δείκτη της σελίδας
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Εκτυπώστε την τιμή του γραμμωτού κώδικα
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Εξάγει γραμμικούς κώδικες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| options | BarcodeOptions | Οι επιλογές για την εξαγωγή γραμμωτών κωδίκων. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)· `null` εάν η εξαγωγή κωδικών barcodes δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε γραμμωτούς κώδικες από την επάνω δεξιά γωνία.

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή γραμμωτών κωδίκων
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Εξάγετε γραμμωτούς κώδικες από την επάνω δεξιά γωνία.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Διατρέξτε τους γραμμωτούς κώδικες
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Εκτυπώστε τον δείκτη της σελίδας
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Εκτυπώστε την τιμή του γραμμωτού κώδικα
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |
| options | BarcodeOptions | Οι επιλογές για την εξαγωγή γραμμωτών κωδίκων. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea)· `null` εάν η εξαγωγή κωδικών barcodes δεν υποστηρίζεται.

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
