---
title: GetImages
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Εξάγει εικόνες από το έγγραφο.
type: docs
weight: 110
url: /el/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Εξάγει εικόνες από το έγγραφο.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) αντικείμενα; `μηδενικό` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή εικόνων από έγγραφα](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Εξαγωγή εικόνων σε αρχεία](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Εξαγωγή εικόνων από έγγραφα του Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Εξαγωγή εικόνων από υπολογιστικά φύλλα του Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Εξαγωγή εικόνων από παρουσιάσεις του Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Εξαγωγή εικόνων από μηνύματα ηλεκτρονικού ταχυδρομείου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Εξαγωγή εικόνων από έγγραφα PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε όλες τις εικόνες από ολόκληρο το έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Εξαγωγή εικόνων
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Ελέγξτε εάν υποστηρίζεται η εξαγωγή εικόνων
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Επανάληψη σε εικόνες
    foreach (PageImageArea image in images)
    {
        // Εκτύπωση ευρετηρίου σελίδας, ορθογωνίου και τύπου εικόνας:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Εξάγει εικόνες από το έγγραφο χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει εικόνες).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή εικόνων. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) αντικείμενα; `μηδενικό` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή εικόνων από έγγραφα](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Εξαγωγή εικόνων σε αρχεία](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Εξαγωγή εικόνων από την περιοχή της σελίδας του εγγράφου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Εξαγωγή εικόνων από έγγραφα του Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Εξαγωγή εικόνων από υπολογιστικά φύλλα του Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Εξαγωγή εικόνων από παρουσιάσεις του Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Εξαγωγή εικόνων από μηνύματα ηλεκτρονικού ταχυδρομείου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Εξαγωγή εικόνων από έγγραφα PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξαγάγετε μόνο εικόνες από την επάνω αριστερή γωνία:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή εικόνων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Εξαγωγή εικόνων από την επάνω αριστερή γωνία μιας σελίδας:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Ελέγξτε εάν υποστηρίζεται η εξαγωγή εικόνων
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Επανάληψη σε εικόνες
    foreach (PageImageArea image in images)
    {
        // Εκτύπωση ευρετηρίου σελίδας, ορθογωνίου και τύπου εικόνας:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Εξάγει εικόνες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) αντικείμενα; `μηδενικό` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή εικόνων από έγγραφα](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Εξαγωγή εικόνων σε αρχεία](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Εξαγωγή εικόνων από τη σελίδα εγγράφου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Εξαγωγή εικόνων από έγγραφα του Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Εξαγωγή εικόνων από υπολογιστικά φύλλα του Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Εξαγωγή εικόνων από παρουσιάσεις του Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Εξαγωγή εικόνων από μηνύματα ηλεκτρονικού ταχυδρομείου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Εξαγωγή εικόνων από έγγραφα PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Παραδείγματα

Για την εξαγωγή εικόνων από μια σελίδα εγγράφου χρησιμοποιείται η ακόλουθη μέθοδος:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή εικόνων
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Εκτύπωση αριθμού σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Επανάληψη σε εικόνες
        // Αγνοούμε τον μηδενικό έλεγχο, καθώς έχουμε ελέγξει νωρίτερα την υποστήριξη της δυνατότητας εξαγωγής εικόνων
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Εκτύπωση ορθογωνίου και τύπου εικόνας
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Εξάγει εικόνες από τη σελίδα του εγγράφου χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει εικόνες).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή εικόνων. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) αντικείμενα; `μηδενικό` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή εικόνων από έγγραφα](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Εξαγωγή εικόνων σε αρχεία](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Εξαγωγή εικόνων από τη σελίδα εγγράφου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Εξαγωγή εικόνων από την περιοχή της σελίδας του εγγράφου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Εξαγωγή εικόνων από έγγραφα του Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Εξαγωγή εικόνων από υπολογιστικά φύλλα του Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Εξαγωγή εικόνων από παρουσιάσεις του Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Εξαγωγή εικόνων από μηνύματα ηλεκτρονικού ταχυδρομείου](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Εξαγωγή εικόνων από έγγραφα PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
