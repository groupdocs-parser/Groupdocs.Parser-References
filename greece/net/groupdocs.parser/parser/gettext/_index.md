---
title: GetText
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Εξάγει ένα κείμενο από το έγγραφο.
type: docs
weight: 150
url: /el/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Εξάγει ένα κείμενο από το έγγραφο.

```csharp
public TextReader GetText()
```

### Επιστρεφόμενη Αξία

Ένα στιγμιότυπο τουTextReader τάξη με το εξαγόμενο κείμενο; `μηδενικό` εάν η εξαγωγή κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή κειμένου από έγγραφα](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Εξαγωγή κειμένου σε Ακριβή λειτουργία](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε ένα κείμενο από ένα έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Εξαγωγή κειμένου στον αναγνώστη
    using(TextReader reader = parser.GetText())
    {
        // Εκτύπωση κειμένου από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι μηδενικός
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Εξάγει μια σελίδα κειμένου από το έγγραφο χρησιμοποιώντας επιλογές κειμένου (για να ενεργοποιηθεί η λειτουργία εξαγωγής ακατέργαστου κειμένου).

```csharp
public TextReader GetText(TextOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | TextOptions | Οι επιλογές εξαγωγής κειμένου. |

### Επιστρεφόμενη Αξία

Ένα στιγμιότυπο τουTextReader τάξη με το εξαγόμενο κείμενο; `μηδενικό` εάν η εξαγωγή κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή κειμένου σε Ακριβή λειτουργία](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Εξαγωγή κειμένου σε λειτουργία Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε ένα ακατέργαστο κείμενο από ένα έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Εξαγωγή ακατέργαστου κειμένου στον αναγνώστη
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Εκτύπωση κειμένου από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι μηδενικός
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Εξάγει ένα κείμενο από τη σελίδα του εγγράφου.

```csharp
public TextReader GetText(int pageIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |

### Επιστρεφόμενη Αξία

Ένα στιγμιότυπο τουTextReader τάξη με το εξαγόμενο κείμενο; `μηδενικό` εάν η εξαγωγή σελίδας κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή κειμένου σε Ακριβή λειτουργία](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε ένα κείμενο από τη σελίδα του εγγράφου:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή κειμένου
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Εκτύπωση αριθμού σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Εξαγωγή κειμένου στον αναγνώστη
        using(TextReader reader = parser.GetText(p))
        {
            // Εκτύπωση κειμένου από το έγγραφο
            // Αγνοούμε τον μηδενικό έλεγχο, καθώς έχουμε ελέγξει την υποστήριξη της δυνατότητας εξαγωγής κειμένου νωρίτερα
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Εξάγει ένα κείμενο από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές κειμένου (για την ενεργοποίηση της λειτουργίας γρήγορης εξαγωγής ακατέργαστου κειμένου).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Το ευρετήριο σελίδας που βασίζεται σε μηδέν. |
| options | TextOptions | Οι επιλογές εξαγωγής κειμένου. |

### Επιστρεφόμενη Αξία

Ένα στιγμιότυπο τουTextReader τάξη με το εξαγόμενο κείμενο; `μηδενικό` εάν η εξαγωγή σελίδας κειμένου δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Εξαγωγή κειμένου σε Ακριβή λειτουργία](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Εξαγωγή κειμένου σε λειτουργία Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εξαγάγετε ένα ακατέργαστο κείμενο από τη σελίδα του εγγράφου:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Ελέγξτε εάν το έγγραφο υποστηρίζει την εξαγωγή κειμένου
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Λάβετε τις πληροφορίες του εγγράφου
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Ελέγξτε εάν το έγγραφο έχει σελίδες
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Επανάληψη σε σελίδες
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Εκτύπωση αριθμού σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Εξαγωγή κειμένου στον αναγνώστη
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Εκτύπωση κειμένου από το έγγραφο
            // Αγνοούμε τον μηδενικό έλεγχο, καθώς έχουμε ελέγξει την υποστήριξη της δυνατότητας εξαγωγής κειμένου νωρίτερα
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
