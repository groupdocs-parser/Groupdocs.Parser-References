---
title: "Search"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αναζητά μια λέξη-κλειδί στο έγγραφο."
type: docs
weight: 250
url: /el/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Αναζητά μια *keyword* στο έγγραφο.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| λέξη-κλειδί | String | Η λέξη-κλειδί για αναζήτηση. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null` εάν η αναζήτηση δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να βρείτε μια λέξη-κλειδί σε ένα έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Αναζητήστε μια λέξη-κλειδί:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Ελέγξτε αν η αναζήτηση υποστηρίζεται
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Επανάληψη στα αποτελέσματα αναζήτησης
    foreach(SearchResult s in sr)
    {
        // Εκτύπωση δείκτη και του ευρεθέντος κειμένου:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Αναζητά μια *keyword* στο έγγραφο χρησιμοποιώντας επιλογές αναζήτησης (κανονική έκφραση, διάκριση πεζών-κεφαλαίων κ.λπ.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| λέξη-κλειδί | String | Η λέξη-κλειδί για αναζήτηση. |
| options | SearchOptions | Οι επιλογές αναζήτησης. |

### Τιμή επιστροφής

Μια συλλογή από αντικείμενα [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null` εάν η αναζήτηση δεν υποστηρίζεται.

### Σχόλια

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να κάνετε αναζήτηση με κανονική έκφραση σε ένα έγγραφο:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Αναζήτηση με κανονική έκφραση με ταίριασμα πεζών/κεφαλαίων
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Ελέγξτε αν η αναζήτηση υποστηρίζεται
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Επανάληψη στα αποτελέσματα αναζήτησης
    foreach(SearchResult s in sr)
    {
        // Εκτύπωση δείκτη και του ευρεθέντος κειμένου:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

Το παρακάτω παράδειγμα δείχνει πώς να αναζητήσετε κείμενο σε σελίδες:

```csharp
// Δημιουργήστε μια παρουσία της κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Αναζήτηση λέξης-κλειδί με αριθμούς σελίδων
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Ελέγξτε αν η αναζήτηση υποστηρίζεται
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Επανάληψη στα αποτελέσματα αναζήτησης
    foreach(SearchResult s in sr)
    {
        // Εκτύπωση δείκτη, αριθμού σελίδας και του ευρεθέντος κειμένου:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
