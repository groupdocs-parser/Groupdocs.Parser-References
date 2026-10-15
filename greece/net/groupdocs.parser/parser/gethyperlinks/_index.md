---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει υπερσυνδέσμους από το έγγραφο."
type: docs
weight: 120
url: /el/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

Εξάγει υπερσυνδέσμους από το έγγραφο.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλους τους υπερσυνδέσμους από ολόκληρο το έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Εξάγετε υπερσυνδέσμους από το έγγραφο
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Διατρέξτε τους υπερσυνδέσμους
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Εκτυπώστε το κείμενο του υπερσυνδέσμου
        Console.WriteLine(h.Text);
        // Εκτυπώστε το URL του υπερσυνδέσμου
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε υπερσυνδέσμους από τη σελίδα του εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Αποκτήστε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε αν το έγγραφο έχει σελίδες
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Διατρέξτε τις σελίδες
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Εξάγετε υπερσυνδέσμους από τη σελίδα του εγγράφου
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Διατρέξτε τους υπερσυνδέσμους
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Εκτυπώστε το κείμενο του υπερσυνδέσμου
            Console.WriteLine(h.Text);
            // Εκτυπώστε το URL του υπερσυνδέσμου
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Εξάγει υπερσυνδέσμους από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει υπερσυνδέσμους).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή υπερσυνδέσμων. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε υπερσυνδέσμους από την περιοχή της σελίδας του εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή υπερσυνδέσμων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Εξάγετε υπερσυνδέσμους από την περιοχή της σελίδας του εγγράφου
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Διατρέξτε τους υπερσυνδέσμους
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Εκτυπώστε το κείμενο του υπερσυνδέσμου
        Console.WriteLine(h.Text);
        // Εκτυπώστε το URL του υπερσυνδέσμου
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει υπερσυνδέσμους).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή υπερσυνδέσμων. |

### Τιμή επιστροφής

Μια συλλογή αντικειμένων [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε υπερσυνδέσμους από την περιοχή σελίδας του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει την εξαγωγή υπερσυνδέσμων
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Αποκτήστε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε αν το έγγραφο έχει σελίδες
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή υπερσυνδέσμων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Διατρέξτε τις σελίδες
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Εξάγετε υπερσυνδέσμους από την περιοχή της σελίδας του εγγράφου
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Διατρέξτε τους υπερσυνδέσμους
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Εκτυπώστε το κείμενο του υπερσυνδέσμου
            Console.WriteLine(h.Text);
            // Εκτυπώστε το URL του υπερσυνδέσμου
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Δείτε επίσης

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
