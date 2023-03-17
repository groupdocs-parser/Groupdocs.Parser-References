---
title: Search
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Αναζητήσεις αkeyword στο έγγραφο.
type: docs
weight: 200
url: /el/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Αναζητήσεις α*keyword* στο έγγραφο.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| keyword | String | Η λέξη-κλειδί για αναζήτηση. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`SearchResult`](../../../groupdocs.parser.data/searchresult) αντικείμενα? `μηδενικό` εάν η αναζήτηση δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Αναζήτηση κειμένου](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Αναζήτηση κειμένου σε έγγραφα του Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Αναζήτηση κειμένου σε υπολογιστικά φύλλα του Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Αναζήτηση κειμένου σε παρουσιάσεις του Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Αναζήτηση κειμένου σε έγγραφα PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Αναζήτηση κειμένου στα μηνύματα ηλεκτρονικού ταχυδρομείου](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Αναζήτηση κειμένου σε ηλεκτρονικά βιβλία EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Αναζήτηση κειμένου σε έγγραφα HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Αναζήτηση κειμένου στις ενότητες του Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να βρείτε μια λέξη-κλειδί σε ένα έγγραφο:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Αναζήτηση λέξης-κλειδιού:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Ελέγξτε εάν υποστηρίζεται η αναζήτηση
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Επανάληψη στα αποτελέσματα αναζήτησης
    foreach(SearchResult s in sr)
    {
        // Εκτυπώστε ένα ευρετήριο και βρέθηκε κείμενο:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Αναζητήσεις α*keyword*στο έγγραφο χρησιμοποιώντας επιλογές αναζήτησης (κανονική έκφραση, περίπτωση αντιστοίχισης κ.λπ.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| keyword | String | Η λέξη-κλειδί για αναζήτηση. |
| options | SearchOptions | Οι επιλογές αναζήτησης. |

### Επιστρεφόμενη Αξία

Μια συλλογή από[`SearchResult`](../../../groupdocs.parser.data/searchresult) αντικείμενα; `μηδενικό` εάν η αναζήτηση δεν υποστηρίζεται.

### Παρατηρήσεις

**Μάθε περισσότερα:**

* [Αναζήτηση κειμένου](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Αναζήτηση κειμένου σε έγγραφα του Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Αναζήτηση κειμένου σε υπολογιστικά φύλλα του Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Αναζήτηση κειμένου σε παρουσιάσεις του Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Αναζήτηση κειμένου σε έγγραφα PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Αναζήτηση κειμένου στα μηνύματα ηλεκτρονικού ταχυδρομείου](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Αναζήτηση κειμένου σε ηλεκτρονικά βιβλία EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Αναζήτηση κειμένου σε έγγραφα HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Αναζήτηση κειμένου στις ενότητες του Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να κάνετε αναζήτηση με μια τυπική έκφραση σε ένα έγγραφο:

Το ακόλουθο παράδειγμα δείχνει πώς να αναζητήσετε ένα κείμενο σε σελίδες:

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Αναζήτηση με κανονική έκφραση με αντιστοίχιση πεζών-κεφαλαίων
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Ελέγξτε εάν υποστηρίζεται η αναζήτηση
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Επανάληψη στα αποτελέσματα αναζήτησης
    foreach(SearchResult s in sr)
    {
        // Εκτυπώστε ένα ευρετήριο και βρέθηκε κείμενο:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Δημιουργία μιας παρουσίας κλάσης Parser
using(Parser parser = new Parser(filePath))
{
    // Αναζήτηση λέξης-κλειδιού με αριθμούς σελίδων
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Ελέγξτε εάν υποστηρίζεται η αναζήτηση
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Επανάληψη στα αποτελέσματα αναζήτησης
    foreach(SearchResult s in sr)
    {
        // Εκτύπωση ευρετηρίου, αριθμού σελίδας και κειμένου που βρέθηκε:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* χώρος ονομάτων [GroupDocs.Parser](../../parser)
* συνέλευση [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
