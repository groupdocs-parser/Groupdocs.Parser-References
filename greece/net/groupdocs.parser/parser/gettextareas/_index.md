---
title: "GetTextAreas"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει περιοχές κειμένου από το έγγραφο."
type: docs
weight: 190
url: /el/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

Εξάγει περιοχές κειμένου από το έγγραφο.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις περιοχές κειμένου από ολόκληρο το έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Εξαγωγή περιοχών κειμένου
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Έλεγχος εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Επανάληψη στις περιοχές κειμένου της σελίδας
    foreach(PageTextArea a in areas)
    {
        // Εκτύπωση δείκτη σελίδας, ορθογωνίου και τιμής περιοχής κειμένου:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Εξάγει περιοχές κειμένου από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, διάκριση πεζών-κεφαλαίων κ.λπ.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| options | PageTextAreaOptions | Οι επιλογές για εξαγωγή περιοχών κειμένου. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε μόνο περιοχές κειμένου με ψηφία από την επάνω αριστερή γωνία:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Δημιουργία των επιλογών που χρησιμοποιούνται για την εξαγωγή περιοχών κειμένου
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Εξαγωγή περιοχών κειμένου που περιέχουν μόνο ψηφία από την επάνω αριστερή γωνία μιας σελίδας:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Έλεγχος εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Επανάληψη στις περιοχές κειμένου της σελίδας
    foreach(PageTextArea a in areas)
    {
        // Εκτύπωση δείκτη σελίδας, ορθογωνίου και τιμής περιοχής κειμένου:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Παραδείγματα

Για την εξαγωγή περιοχών κειμένου από μια σελίδα εγγράφου χρησιμοποιείται η παρακάτω μέθοδος:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Έλεγχος εάν το έγγραφο υποστηρίζει εξαγωγή περιοχών κειμένου
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Αποκτήστε τις πληροφορίες του εγγράφου
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Ελέγξτε αν το έγγραφο έχει σελίδες
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Διατρέξτε τις σελίδες
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Επανάληψη στις περιοχές κειμένου της σελίδας
        // Αγνοούμε τον έλεγχο null καθώς έχουμε ήδη ελέγξει την υποστήριξη της λειτουργίας εξαγωγής περιοχών κειμένου νωρίτερα
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Εκτύπωση ορθογωνίου και τιμής περιοχής κειμένου:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, διάκριση πεζών-κεφαλαίων κ.λπ.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |
| options | PageTextAreaOptions | Οι επιλογές για εξαγωγή περιοχών κειμένου. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null` εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
