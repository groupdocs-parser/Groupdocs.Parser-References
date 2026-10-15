---
title: "GetImages"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει εικόνες από το έγγραφο."
type: docs
weight: 130
url: /el/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

Εξάγει εικόνες από το έγγραφο.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)· `null` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις εικόνες από ολόκληρο το έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Εξάγετε εικόνες
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Έλεγχος εάν η εξαγωγή εικόνων υποστηρίζεται
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Επανάληψη πάνω από τις εικόνες
    foreach (PageImageArea image in images)
    {
        // Εκτυπώστε τον δείκτη σελίδας, το ορθογώνιο και τον τύπο εικόνας:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Εξάγει εικόνες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει εικόνες).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή εικόνων. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)· `null` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε μόνο εικόνες από την επάνω αριστερή γωνία:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Δημιουργήστε τις επιλογές που χρησιμοποιούνται για την εξαγωγή εικόνων
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Εξαγωγή εικόνων από την επάνω αριστερή γωνία μιας σελίδας:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Έλεγχος εάν η εξαγωγή εικόνων υποστηρίζεται
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Επανάληψη πάνω από τις εικόνες
    foreach (PageImageArea image in images)
    {
        // Εκτυπώστε τον δείκτη σελίδας, το ορθογώνιο και τον τύπο εικόνας:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Εξάγει εικόνες από τη σελίδα του εγγράφου.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)· `null` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Παραδείγματα

Για την εξαγωγή εικόνων από μια σελίδα εγγράφου χρησιμοποιείται η ακόλουθη μέθοδος:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using (Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει εξαγωγή εικόνων
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Επανάληψη πάνω από τις εικόνες
        // Αγνοούμε τον έλεγχο null καθώς έχουμε ήδη ελέγξει την υποστήριξη της λειτουργίας εξαγωγής εικόνων
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Εκτυπώστε ένα ορθογώνιο και τον τύπο εικόνας
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Εξάγει εικόνες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει εικόνες).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |
| options | PageAreaOptions | Οι επιλογές για την εξαγωγή εικόνων. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)· `null` εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Δείτε επίσης

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
