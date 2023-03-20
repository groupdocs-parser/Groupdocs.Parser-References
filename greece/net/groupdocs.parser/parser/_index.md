---
title: Parser
second_title: GroupDocs.Parser για Αναφορά API .NET
description: Αντιπροσωπεύει την κύρια κλάση που ελέγχει το κείμενο τις εικόνες την εξαγωγή κοντέινερ και τη λειτουργία ανάλυσης.
type: docs
weight: 640
url: /el/net/groupdocs.parser/parser/
---
## Parser class

Αντιπροσωπεύει την κύρια κλάση που ελέγχει το κείμενο, τις εικόνες, την εξαγωγή κοντέινερ και τη λειτουργία ανάλυσης.

```csharp
public sealed class Parser : IDisposable
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) κλάση για εξαγωγή δεδομένων από μια βάση δεδομένων. |
| [Parser](parser#constructor)(EmailConnection) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) κλάση για εξαγωγή δεδομένων από απομακρυσμένο διακομιστή email. |
| [Parser](parser#constructor_4)(Stream) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη. |
| [Parser](parser#constructor_8)(string) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) κλάση για εξαγωγή δεδομένων από μια βάση δεδομένων. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) κλάση για εξαγωγή δεδομένων από απομακρυσμένο διακομιστή email. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη με[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη με[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη με[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη με[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη με[`LoadOptions`](../../groupdocs.parser.options/loadoptions) και[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Αρχικοποιεί μια νέα παρουσία του[`Parser`](../parser) τάξη με[`LoadOptions`](../../groupdocs.parser.options/loadoptions) και[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Αποκτά τις υποστηριζόμενες δυνατότητες. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Εκτελεί εργασίες που καθορίζονται από την εφαρμογή που σχετίζονται με την απελευθέρωση, την απελευθέρωση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Λήψη προεπισκόπησης σελίδων. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Εξάγει γραμμικούς κώδικες από το έγγραφο. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Εξάγει γραμμικούς κώδικες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει γραμμικούς κώδικες). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει γραμμικούς κώδικες). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Εξάγει ένα αντικείμενο κοντέινερ από το έγγραφο για να εργαστεί με μορφές που περιέχουν συνημμένα, αρχεία ZIP κ.λπ. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Επιστρέφει τις γενικές πληροφορίες για το έγγραφο. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Εξάγει ένα μορφοποιημένο κείμενο από το έγγραφο. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Εξάγει ένα μορφοποιημένο κείμενο από τη σελίδα του εγγράφου. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Εξάγει μια επισήμανση από το έγγραφο. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Εξάγει υπερσυνδέσμους από το έγγραφο. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Εξάγει υπερσυνδέσμους από το έγγραφο χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει υπερσυνδέσμους). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει υπερσυνδέσμους). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Εξάγει εικόνες από το έγγραφο. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Εξάγει εικόνες από τη σελίδα του εγγράφου. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Εξάγει εικόνες από το έγγραφο χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει εικόνες). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Εξάγει εικόνες από τη σελίδα του εγγράφου χρησιμοποιώντας τις επιλογές προσαρμογής (για να ορίσετε την ορθογώνια περιοχή που περιέχει εικόνες). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Εξάγει μεταδεδομένα από το έγγραφο. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Εξάγει ένα δομημένο κείμενο από το έγγραφο. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Εξάγει πίνακες από το έγγραφο. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Εξάγει πίνακες από τη σελίδα του εγγράφου. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Εξάγει ένα κείμενο από το έγγραφο. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Εξάγει ένα κείμενο από τη σελίδα του εγγράφου. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Εξάγει μια σελίδα κειμένου από το έγγραφο χρησιμοποιώντας επιλογές κειμένου (για να ενεργοποιηθεί η λειτουργία εξαγωγής ακατέργαστου κειμένου). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Εξάγει ένα κείμενο από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές κειμένου (για την ενεργοποίηση της λειτουργίας γρήγορης εξαγωγής ακατέργαστου κειμένου). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Εξάγει περιοχές κειμένου από το έγγραφο. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Εξάγει περιοχές κειμένου από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, κεφαλαία αντιστοίχισης, κ.λπ.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, κεφαλαία αντιστοίχισης κ.λπ.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Εξάγει έναν πίνακα περιεχομένων από το έγγραφο. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Αναλύει το έγγραφο από το πρότυπο που δημιουργείται από το χρήστη. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Αναλύει τη φόρμα εγγράφου. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Αναζητήσεις α*keyword* στο έγγραφο. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Αναζητήσεις α*keyword*στο έγγραφο χρησιμοποιώντας επιλογές αναζήτησης (κανονική έκφραση, περίπτωση αντιστοίχισης κ.λπ.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Parser](../../groupdocs.parser)
* συνέλευση [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
