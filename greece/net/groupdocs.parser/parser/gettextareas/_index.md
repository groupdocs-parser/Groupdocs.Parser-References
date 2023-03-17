---
title: GetTextAreas
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Εξάγει περιοχές κειμένου από το έγγραφο.
type: docs
weight: 160
url: /el/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Εξάγει περιοχές κειμένου από το έγγραφο.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή περιοχών κειμένου](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις περιοχές κειμένου από ολόκληρο το έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Εξαγωγή περιοχών κειμένου
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Ελέγξτε εάν υποστηρίζεται η εξαγωγή περιοχών κειμένου
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Επανάληψη περιοχών κειμένου σελίδας
    foreach(PageTextArea a in areas)
    {
        // Εκτύπωση τιμής ευρετηρίου σελίδας, ορθογωνίου και περιοχής κειμένου:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Εξάγει περιοχές κειμένου από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, κεφαλαία αντιστοίχισης, κ.λπ.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PageTextAreaOptions | Οι επιλογές για εξαγωγή περιοχής κειμένου. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή περιοχών κειμένου](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε μόνο περιοχές κειμένου με ψηφία από την επάνω αριστερή γωνία:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή της περιοχής κειμένου
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Εξαγωγή περιοχών κειμένου που περιέχουν μόνο ψηφία από την επάνω αριστερή γωνία μιας σελίδας:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Ελέγξτε εάν υποστηρίζεται η εξαγωγή περιοχών κειμένου
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Επανάληψη περιοχών κειμένου σελίδας
    foreach(PageTextArea a in areas)
    {
        // Εκτύπωση τιμής ευρετηρίου σελίδας, ορθογωνίου και περιοχής κειμένου:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή περιοχών κειμένου](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Παραδείγματα

Για την εξαγωγή περιοχών κειμένου από μια σελίδα εγγράφου χρησιμοποιείται η ακόλουθη μέθοδος:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή περιοχών κειμένου
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Λάβετε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε εάν το έγγραφο έχει σελίδες
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Επανάληψη σε σελίδες
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Εκτύπωση αριθμού σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Επανάληψη περιοχών κειμένου σελίδας
        // Αγνοούμε τον μηδενικό έλεγχο καθώς έχουμε ελέγξει νωρίτερα την υποστήριξη δυνατοτήτων εξαγωγής περιοχών κειμένου
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Εκτύπωση τιμής ορθογωνίου και περιοχής κειμένου:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, κεφαλαία αντιστοίχισης κ.λπ.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |
| options | PageTextAreaOptions | Οι επιλογές για εξαγωγή περιοχής κειμένου. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) αντικείμενα; `μηδενικό` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή περιοχών κειμένου](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
