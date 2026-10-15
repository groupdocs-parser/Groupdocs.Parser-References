---
title: "GetText"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει κείμενο από το έγγραφο."
type: docs
weight: 180
url: /el/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Εξάγει κείμενο από το έγγραφο.

```csharp
public TextReader GetText()
```

### Τιμή επιστροφής

Μία παρουσία της κλάσης TextReader με το εξαγόμενο κείμενο· `null` εάν η εξαγωγή κειμένου δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε κείμενο από ένα έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Εξάγετε κείμενο στον αναγνώστη
    using(TextReader reader = parser.GetText())
    {
        // Εκτυπώστε κείμενο από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Εξάγει μια σελίδα κειμένου από το έγγραφο χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου).

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| options | TextOptions | Οι επιλογές εξαγωγής κειμένου. |

### Τιμή επιστροφής

Μία παρουσία της κλάσης TextReader με το εξαγόμενο κείμενο· `null` εάν η εξαγωγή κειμένου δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε ακατέργαστο κείμενο από ένα έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Εξάγετε ακατέργαστο κείμενο στον αναγνώστη
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Εκτυπώστε κείμενο από το έγγραφο
        // Εάν η εξαγωγή κειμένου δεν υποστηρίζεται, ο αναγνώστης είναι null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Δείτε επίσης

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Εξάγει κείμενο από τη σελίδα του εγγράφου.

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |

### Τιμή επιστροφής

Μία παρουσία της κλάσης TextReader με το εξαγόμενο κείμενο· `null` εάν η εξαγωγή κειμένου σε σελίδα δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε κείμενο από τη σελίδα του εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει εξαγωγή κειμένου
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Εξάγετε κείμενο στον αναγνώστη
        using(TextReader reader = parser.GetText(p))
        {
            // Εκτυπώστε κείμενο από το έγγραφο
            // Αγνοούμε τον έλεγχο null καθώς έχουμε ελέγξει νωρίτερα την υποστήριξη της λειτουργίας εξαγωγής κειμένου
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Εξάγει κείμενο από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| pageIndex | Int32 | Ο δείκτης σελίδας με βάση το μηδέν. |
| options | TextOptions | Οι επιλογές εξαγωγής κειμένου. |

### Τιμή επιστροφής

Μία παρουσία της κλάσης TextReader με το εξαγόμενο κείμενο· `null` εάν η εξαγωγή κειμένου σε σελίδα δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε ακατέργαστο κείμενο από τη σελίδα του εγγράφου:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Ελέγξτε αν το έγγραφο υποστηρίζει εξαγωγή κειμένου
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Αποκτήστε τις πληροφορίες του εγγράφου
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Ελέγξτε αν το έγγραφο έχει σελίδες
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Διατρέξτε τις σελίδες
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Εκτυπώστε έναν αριθμό σελίδας 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Εξάγετε κείμενο στον αναγνώστη
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Εκτυπώστε κείμενο από το έγγραφο
            // Αγνοούμε τον έλεγχο null καθώς έχουμε ελέγξει νωρίτερα την υποστήριξη της λειτουργίας εξαγωγής κειμένου
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Δείτε επίσης

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
