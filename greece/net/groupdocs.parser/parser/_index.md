---
title: "Αναλυτής"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Αντιπροσωπεύει την κύρια κλάση που ελέγχει την εξαγωγή περιεχομένου εικόνων κειμένου και τη λειτουργικότητα ανάλυσης."
type: docs
weight: 30
url: /el/net/groupdocs.parser/parser/
---

## Parser class

Αντιπροσωπεύει την κύρια κλάση που ελέγχει το κείμενο, τις εικόνες, την εξαγωγή περιεχομένου και τη λειτουργικότητα ανάλυσης.

```csharp
public sealed class Parser : IDisposable
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από μια βάση δεδομένων. |
| [Parser](parser#constructor)(EmailConnection) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από απομακρυσμένο διακομιστή email. |
| [Parser](parser#constructor_4)(Stream) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser). |
| [Parser](parser#constructor_8)(string) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser). |
| [Parser](parser#constructor_12)(Uri) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από ένα URI. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από μια βάση δεδομένων. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από απομακρυσμένο διακομιστή email. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) με [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) με [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) με [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) με [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από ένα URI με *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από ένα URI με *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) με [`LoadOptions`](../../groupdocs.parser.options/loadoptions) και [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) με [`LoadOptions`](../../groupdocs.parser.options/loadoptions) και [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Parser`](../parser) για την εξαγωγή δεδομένων από ένα URI με *loadOptions* και *parserSettings*. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Λαμβάνει τις υποστηριζόμενες λειτουργίες. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Εκτελεί εργασίες που ορίζονται από την εφαρμογή, σχετικές με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Δημιουργεί πεδία για αυτόματη προσαρμογή της θέσης και της κλίμακας του προτύπου. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Λάβετε προεπισκόπηση των σελίδων. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Εξάγει σημειώσεις από το έγγραφο. Σημειώστε ότι μόνο η μορφή PDF υποστηρίζεται επί του παρόντος. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Εξάγει σημειώσεις από τη σελίδα του εγγράφου. Σημειώστε ότι μόνο η μορφή PDF υποστηρίζεται επί του παρόντος. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Εξάγει γραμμικούς κώδικες από το έγγραφο. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Εξάγει γραμμικούς κώδικες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Εξάγει γραμμικούς κώδικες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Εξάγει ένα αντικείμενο container από το έγγραφο για εργασία με μορφές που περιέχουν συνημμένα, αρχεία ZIP κ.λπ. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Επιστρέφει τις γενικές πληροφορίες για το έγγραφο. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Εξάγει μορφοποιημένο κείμενο από το έγγραφο. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Εξάγει μορφοποιημένο κείμενο από τη σελίδα του εγγράφου. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Εξάγει επισήμανση από το έγγραφο. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Εξάγει υπερσυνδέσμους από το έγγραφο. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Εξάγει υπερσυνδέσμους από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει υπερσυνδέσμους). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει υπερσυνδέσμους). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Εξάγει εικόνες από το έγγραφο. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Εξάγει εικόνες από τη σελίδα του εγγράφου. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Εξάγει εικόνες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει εικόνες). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Εξάγει εικόνες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογώνιου περιοχής που περιέχει εικόνες). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Εξάγει μεταδεδομένα από το έγγραφο. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Δημιουργεί προεπισκόπηση σελίδας εγγράφου. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Δημιουργεί προεπισκόπηση σελίδας εγγράφου χρησιμοποιώντας επιλογές προσαρμογής. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Εξάγει δομημένο κείμενο από το έγγραφο. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Εξάγει πίνακες από το έγγραφο. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Εξάγει πίνακες από τη σελίδα του εγγράφου. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Εξάγει πίνακες από το έγγραφο. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Εξάγει πίνακες από τη σελίδα του εγγράφου. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Εξάγει κείμενο από το έγγραφο. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Εξάγει κείμενο από τη σελίδα του εγγράφου. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Εξάγει μια σελίδα κειμένου από το έγγραφο χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Εξάγει κείμενο από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Εξάγει περιοχές κειμένου από το έγγραφο. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Εξάγει περιοχές κειμένου από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, διάκριση πεζών-κεφαλαίων κ.λπ.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, διάκριση πεζών-κεφαλαίων κ.λπ.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Εξάγει πίνακα περιεχομένων από το έγγραφο. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Εξάγει κελιά φύλλου εργασίας. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Εξάγει κελιά φύλλου εργασίας χρησιμοποιώντας επιλογές προσαρμογής. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Εξάγει τις πληροφορίες για όλα τα φύλλα εργασίας στο λογιστικό φύλλο. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Εξάγει τις πληροφορίες για το φύλλο εργασίας. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Αναλύει το έγγραφο με το πρότυπο που δημιουργήθηκε από τον χρήστη. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Αναλύει το έγγραφο με το πρότυπο που δημιουργήθηκε από τον χρήστη χρησιμοποιώντας επιλογές προσαρμογής. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Επιλέγει το πιο κατάλληλο πρότυπο από τη δοθείσα συλλογή και στη συνέχεια αναλύει το έγγραφο με βάση το επιλεγμένο πρότυπο. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Αναλύει τη φόρμα του εγγράφου. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Αναζητά μια *keyword* στο έγγραφο. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Αναζητά μια *keyword* στο έγγραφο χρησιμοποιώντας επιλογές αναζήτησης (κανονική έκφραση, διάκριση πεζών-κεφαλαίων κ.λπ.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |

### Δείτε επίσης

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
