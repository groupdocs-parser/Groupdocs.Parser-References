---
title: GetHyperlinks
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Εξάγει υπερσυνδέσμους από το έγγραφο.
type: docs
weight: 100
url: /el/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Εξάγει υπερσυνδέσμους από το έγγραφο.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλους τους υπερσυνδέσμους από ολόκληρο το έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Εξαγωγή υπερσυνδέσμων από το έγγραφο
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Επανάληψη σε υπερσυνδέσμους
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Εκτυπώστε το κείμενο υπερσύνδεσης
        Console.WriteLine(h.Text);
        // Εκτυπώστε τη διεύθυνση URL υπερσύνδεσης
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε υπερσυνδέσμους από τη σελίδα του εγγράφου:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
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
        // Εξαγωγή υπερσυνδέσμων από τη σελίδα του εγγράφου
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Επανάληψη σε υπερσυνδέσμους
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Εκτυπώστε το κείμενο υπερσύνδεσης
            Console.WriteLine(h.Text);
            // Εκτυπώστε τη διεύθυνση URL υπερσύνδεσης
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Εξάγει υπερσυνδέσμους από το έγγραφο χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει υπερσυνδέσμους).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή υπερσυνδέσμων. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε υπερσυνδέσμους από την περιοχή της σελίδας του εγγράφου:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή υπερσυνδέσμων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Εξαγωγή υπερσυνδέσμων από την περιοχή της σελίδας του εγγράφου
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Επανάληψη σε υπερσυνδέσμους
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Εκτυπώστε το κείμενο υπερσύνδεσης
        Console.WriteLine(h.Text);
        // Εκτυπώστε τη διεύθυνση URL υπερσύνδεσης
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει υπερσυνδέσμους).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή υπερσυνδέσμων. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε υπερσυνδέσμους από την περιοχή της σελίδας του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Λάβετε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε εάν το έγγραφο έχει σελίδες
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή υπερσυνδέσμων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Επανάληψη σε σελίδες
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Εκτύπωση αριθμού σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Εξαγωγή υπερσυνδέσμων από την περιοχή της σελίδας του εγγράφου
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Επανάληψη σε υπερσυνδέσμους
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Εκτυπώστε το κείμενο υπερσύνδεσης
            Console.WriteLine(h.Text);
            // Εκτυπώστε τη διεύθυνση URL υπερσύνδεσης
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
