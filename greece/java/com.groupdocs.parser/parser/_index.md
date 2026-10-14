---
title: "Parser"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αναπαριστά την κύρια κλάση που ελέγχει την εξαγωγή του περιεχομένου εικόνων κειμένου και τη λειτουργία ανάλυσης."
type: docs
weight: 10
url: /el/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Αντιπροσωπεύει την κύρια κλάση που ελέγχει τη λειτουργία εξαγωγής κειμένου, εικόνων, περιεχομένου και ανάλυσης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL με  loadOptions . |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL με  parserSettings . |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL με  loadOptions  και  parserSettings . |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από μια βάση δεδομένων. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από μια βάση δεδομένων. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions) και το [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions) και το [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο. |
|
|  | [getFeatures()](#getFeatures--) | Λαμβάνει τις υποστηριζόμενες δυνατότητες. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Δημιουργεί μια προεπισκόπηση σελίδας εγγράφου. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Δημιουργεί μια προεπισκόπηση σελίδας εγγράφου χρησιμοποιώντας επιλογές προσαρμογής. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Λάβετε προεπισκόπηση σελίδων. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Επιστρέφει τις γενικές πληροφορίες για το έγγραφο. |
|
|  | [getText()](#getText--) | Εξάγει κείμενο από το έγγραφο. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Εξάγει μια σελίδα κειμένου από το έγγραφο χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου). |
|
|  | [getText(int pageIndex)](#getText-int-) | Εξάγει κείμενο από τη σελίδα του εγγράφου. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Εξάγει κείμενο από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Εξάγει μορφοποιημένο κείμενο από το έγγραφο. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Εξάγει μορφοποιημένο κείμενο από τη σελίδα του εγγράφου. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Αναζητά μια λέξη-κλειδί στο έγγραφο. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Αναζητά μια λέξη-κλειδί στο έγγραφο χρησιμοποιώντας επιλογές αναζήτησης (κανονική έκφραση, ευαίσθητο σε πεζά/κεφαλαία, κ.λπ.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Εξάγει επισήμανση από το έγγραφο. |
|
|  | [getToc()](#getToc--) | Εξάγει πίνακα περιεχομένων από το έγγραφο. |
|
|  | [getMetadata()](#getMetadata--) | Εξάγει μεταδεδομένα από το έγγραφο. |
|
|  | [getAnnotations()](#getAnnotations--) | Εξάγει σχολιασμούς από το έγγραφο. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Εξάγει σχολιασμούς από τη σελίδα του εγγράφου. |
|
|  | [getContainer()](#getContainer--) | Εξάγει ένα αντικείμενο container από το έγγραφο για εργασία με μορφές που περιέχουν συνημμένα, αρχεία ZIP κ.ά. |
|
|  | [getTextAreas()](#getTextAreas--) | Εξάγει περιοχές κειμένου από το έγγραφο. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Εξάγει περιοχές κειμένου από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, ταίριασμα πεζών/κεφαλαίων, κ.λπ.). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, ταίριασμα πεζών/κεφαλαίων, κ.λπ.). |
|
|  | [getImages()](#getImages--) | Εξάγει εικόνες από το έγγραφο. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Εξάγει εικόνες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει εικόνες). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Εξάγει εικόνες από τη σελίδα του εγγράφου. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Εξάγει εικόνες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει εικόνες). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Εξάγει υπερσυνδέσμους από το έγγραφο. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Εξάγει υπερσυνδέσμους από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει υπερσυνδέσμους). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει υπερσυνδέσμους). |
|
|  | [getBarcodes()](#getBarcodes--) | Εξάγει γραμμωτούς κώδικες από το έγγραφο. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Εξάγει γραμμωτούς κώδικες από τη σελίδα του εγγράφου. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Εξάγει γραμμωτούς κώδικες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει γραμμωτούς κώδικες). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Εξάγει γραμμωτούς κώδικες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει γραμμωτούς κώδικες). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Εξάγει πίνακες από το έγγραφο. |
|
|  | [getTables()](#getTables--) | Εξάγει πίνακες από το έγγραφο, εντοπίζοντάς τους αυτόματα. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Εξάγει πίνακες από τη σελίδα του εγγράφου. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Εξάγει πίνακες από τη σελίδα του εγγράφου, εντοπίζοντάς τους αυτόματα. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Δημιουργεί μια συλλογή προσαρμογών [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s για το έγγραφο. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Εξάγει τις πληροφορίες για όλα τα φύλλα εργασίας στο λογιστικό φύλλο. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Εξάγει τις πληροφορίες για το φύλλο εργασίας. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Εξάγει κελιά του φύλλου εργασίας. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Εξάγει κελιά του φύλλου εργασίας χρησιμοποιώντας επιλογές προσαρμογής. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Αναλύει το έγγραφο με το πρότυπο που δημιουργήθηκε από τον χρήστη. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Αναλύει το έγγραφο με το πρότυπο που δημιουργήθηκε από τον χρήστη, με τις παρεχόμενες επιλογές. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Αναλύει το έγγραφο επιλέγοντας αυτόματα το πιο κατάλληλο πρότυπο από μια συλλογή. |
|
|  | [parseForm()](#parseForm--) | Αναλύει τη φόρμα του εγγράφου. |
|
|  | [getStructure()](#getStructure--) | Εξάγει δομημένο κείμενο από το έγγραφο. |
|
|  | [close()](#close--) | Κλείνει αυτόν τον πόρο, απελευθερώνοντας τυχόν υποκείμενους πόρους. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | url | java.net.URL | Το URL στο οποίο αποστέλλεται το αίτημα |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL με  loadOptions .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | url | java.net.URL | Το URL στο οποίο αποστέλλεται το αίτημα. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του αρχείου. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL με  parserSettings .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | url | java.net.URL | Το URL στο οποίο αποστέλλεται το αίτημα. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από ένα URL με  loadOptions  και  parserSettings .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | url | java.net.URL | Το URL στο οποίο αποστέλλεται το αίτημα. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του αρχείου. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από μια βάση δεδομένων.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε δεδομένα από τη βάση δεδομένων Sqlite:

````
// Create DbConnection object
 java.sql.Connection connection = java.sql.DriverManager.getConnection(String.format("jdbc:sqlite:%s", Constants.SampleDatabase));
 // Create an instance of Parser class to extract tables from the database
 try (Parser parser = new Parser(connection)) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     // Check if toc extraction is supported
     if (!parser.getFeatures().isToc()) {
         System.out.println("Toc extraction isn't supported.");
         return;
     }
     // Get a list of tables
     Iterable toc = parser.getToc();
     // Iterate over tables
     for(TocItem i : toc)
     {
         // Print the table name
         System.out.println(i.extractText());
         // Extract a table content as a text
         try(TextReader reader = parser.getText(i.getPageIndex().intValue()))
         {
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | connection | java.sql.Connection | Η σύνδεση βάσης δεδομένων. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) για την εξαγωγή δεδομένων από μια βάση δεδομένων.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε δεδομένα από τη βάση δεδομένων Sqlite:

````
// Create DbConnection object
 java.sql.Connection connection = java.sql.DriverManager.getConnection(String.format("jdbc:sqlite:%s", Constants.SampleDatabase));
 // Create an instance of Parser class to extract tables from the database
 try (Parser parser = new Parser(connection)) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     // Check if toc extraction is supported
     if (!parser.getFeatures().isToc()) {
         System.out.println("Toc extraction isn't supported.");
         return;
     }
     // Get a list of tables
     Iterable toc = parser.getToc();
     // Iterate over tables
     for(TocItem i : toc)
     {
         // Print the table name
         System.out.println(i.extractText());
         // Extract a table content as a text
         try(TextReader reader = parser.getText(i.getPageIndex().intValue()))
         {
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | connection | java.sql.Connection | Η σύνδεση βάσης δεδομένων. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε email από τον Exchange Server:

````
// Create the connection object for Exchange Web Services protocol
 EmailConnection connection = new EmailEwsConnection(
         "https://outlook.office365.com/ews/exchange.asmx",
         "email@server",
         "password");
 // Create an instance of Parser class to extract emails from the remote server
 try (Parser parser = new Parser(connection)) {
     // Check if container extraction is supported
     if (!parser.getFeatures().isContainer()) {
         System.out.println("Container extraction isn't supported.");
         return;
     }
     // Extract email messages from the server
     Iterable emails = parser.getContainer();
     // Iterate over attachments
     for (ContainerItem item : emails) {
         // Create an instance of Parser class for email message
         try (Parser emailParser = item.openParser()) {
             // Extract the email text
             try (TextReader reader = emailParser.getText()) {
                 // Print the email text
                 System.out.println(reader == null ? "Text extraction isn't supported." : reader.readToEnd());
             }
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Η σύνδεση email. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε email από τον Exchange Server:

````
// Create the connection object for Exchange Web Services protocol
 EmailConnection connection = new EmailEwsConnection(
         "https://outlook.office365.com/ews/exchange.asmx",
         "email@server",
         "password");
 // Create an instance of Parser class to extract emails from the remote server
 try (Parser parser = new Parser(connection)) {
     // Check if container extraction is supported
     if (!parser.getFeatures().isContainer()) {
         System.out.println("Container extraction isn't supported.");
         return;
     }
     // Extract email messages from the server
     Iterable emails = parser.getContainer();
     // Iterate over attachments
     for (ContainerItem item : emails) {
         // Create an instance of Parser class for email message
         try (Parser emailParser = item.openParser()) {
             // Extract the email text
             try (TextReader reader = emailParser.getText()) {
                 // Print the email text
                 System.out.println(reader == null ? "Text extraction isn't supported." : reader.readToEnd());
             }
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Η σύνδεση email. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Το παρακάτω παράδειγμα δείχνει πώς να φορτώσετε το έγγραφο από τον τοπικό δίσκο:

````
// Set the filePath
 String filePath = Constants.SamplePdf;
 // Create an instance of Parser class with the filePath
 try (Parser parser = new Parser(filePath)) {
     // Extract a text into the reader
     try (TextReader reader = parser.getText()) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Ο κωδικός πρόσβασης του εγγράφου περνιέται από την κλάση [LoadOptions](../../com.groupdocs.parser.options/loadoptions):

````
try {
     String password = "123456";
     // Create an instance of Parser class with the password:
     try (Parser parser = new Parser(Constants.SamplePassword, new LoadOptions(password))) {
         // Check if text extraction is supported
         if (!parser.getFeatures().isText()) {
             System.out.println("Text extraction isn't supported.");
             return;
         }
         // Print the document text
         try (TextReader reader = parser.getText()) {
             System.out.println(reader.readToEnd());
         }
     }
 } catch (InvalidPasswordException ex) {
     // Print the message if the password is incorrect or empty
     System.out.println("Invalid password");
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του αρχείου. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions) και το [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε τις πληροφορίες μέσω της διεπαφής [ILogger](../../com.groupdocs.parser.options/ilogger):

````
try {
     // Create an instance of Logger class
     Logger logger = new Logger();
     // Create an instance of Parser class with the parser settings
     try (Parser parser = new Parser(Constants.SamplePassword, null, new ParserSettings(logger))) {
         // Check if text extraction is supported
         if (!parser.getFeatures().isText()) {
             System.out.println("Text extraction isn't supported.");
             return;
         }
         // Print the document text
         try (TextReader reader = parser.getText()) {
             System.out.println(reader.readToEnd());
         }
     }
 } catch (InvalidPasswordException | IOException ex) {
     ; // Ignore the exception
 }

 class Logger implements ILogger {
     public void error(String message, Exception exception) {
         // Print error message
         System.out.println("Error: " + message);
     }

     public void trace(String message) {
         // Print event message
         System.out.println("Event: " + message);
     }

     public void warning(String message) {
         // Print warning message
         System.out.println("Warning: " + message);
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του αρχείου. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Το παρακάτω παράδειγμα δείχνει πώς να φορτώσετε το έγγραφο από τη ροή:

````
// Create the stream
 try (InputStream stream = new FileInputStream(Constants.SamplePdf)) {
     // Create an instance of Parser class with the stream
     try (Parser parser = new Parser(stream)) {
         // Extract a text into the reader
         try (TextReader reader = parser.getText()) {
             // Print a text from the document
             // If text extraction isn't supported, a reader is null
             System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Η ροή εισόδου προέλευσης. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Σε ορισμένες περιπτώσεις είναι απαραίτητο να οριστεί το [FileFormat](../../com.groupdocs.parser.options/fileformat). Και για ειδικές περιπτώσεις (βάσεις δεδομένων, διακομιστής email)
και για την ανίχνευση τύπων αρχείων με βάση το περιεχόμενο:

````
// Create an instance of Parser class for markdown document
 try (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup))) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     try (TextReader reader = parser.getText()) {
         // Print the document text
         // Markdown is detected; text without special symbols is printed
         System.out.println(reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Η ροή εισόδου προέλευσης. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του αρχείου. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Η ροή εισόδου προέλευσης. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Parser](../../com.groupdocs.parser/parser) με το [LoadOptions](../../com.groupdocs.parser.options/loadoptions) και το [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε τις πληροφορίες μέσω της διεπαφής [ILogger](../../com.groupdocs.parser.options/ilogger):

````
try {
     // Create an instance of Logger class
     Logger logger = new Logger();
     // Create an instance of Parser class with the parser settings
     try (Parser parser = new Parser(Constants.SamplePassword, null, new ParserSettings(logger))) {
         // Check if text extraction is supported
         if (!parser.getFeatures().isText()) {
             System.out.println("Text extraction isn't supported.");
             return;
         }
         // Print the document text
         try (TextReader reader = parser.getText()) {
             System.out.println(reader.readToEnd());
         }
     }
 } catch (InvalidPasswordException | IOException ex) {
     ; // Ignore the exception
 }

 class Logger implements ILogger {
     public void error(String message, Exception exception) {
         // Print error message
         System.out.println("Error: " + message);
     }

     public void trace(String message) {
         // Print event message
         System.out.println("Event: " + message);
     }

     public void warning(String message) {
         // Print warning message
         System.out.println("Warning: " + message);
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Η ροή εισόδου προέλευσης. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του αρχείου. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο.

Ο παρακάτω κώδικας δείχνει πώς να ελέγξετε αν ένα αρχείο είναι προστατευμένο με κωδικό πρόσβασης:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Επιστρέφει τις γενικές πληροφορίες για ένα αρχείο.

Ο παρακάτω κώδικας δείχνει πώς να ελέγξετε αν ένα αρχείο είναι προστατευμένο με κωδικό πρόσβασης:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Η ροή εισόδου προέλευσης. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Λαμβάνει τις υποστηριζόμενες δυνατότητες.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Εάν η δυνατότητα δεν υποστηρίζεται, η μέθοδος επιστρέφει
null
αντί για την τιμή. Ορισμένες λειτουργίες μπορεί να καταναλώσουν
σημαντικό χρόνο. Έτσι δεν είναι βέλτιστο να καλέσετε τη μέθοδο μόνο για να ελέγξετε την υποστήριξη της δυνατότητας.
Για αυτό το σκοπό χρησιμοποιείται η ιδιότητα Features:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Check if text extraction is supported for the document
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported");
         return;
     }
     // Extract a text from the document
     try (TextReader reader = parser.getText()) {
         System.out.println(reader.readToEnd());
     }
 }
 
````



**Returns:**
[Features](../../com.groupdocs.parser.options/features) - An instance of [Features](../../com.groupdocs.parser.options/features) class that represents the supported features.

### getPagePreview(int pageIndex) {#getPagePreview-int-}
```
public OutputStream getPagePreview(int pageIndex)
```


Δημιουργεί μια προεπισκόπηση σελίδας εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.io.OutputStream - Μία παρουσία του java.io.OutputStream που περιέχει μια εικόνα της σελίδας του εγγράφου·  null  εάν η δημιουργία προεπισκόπησης σελίδας δεν υποστηρίζεται.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Δημιουργεί μια προεπισκόπηση σελίδας εγγράφου χρησιμοποιώντας επιλογές προσαρμογής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Οι επιλογές για την προσαρμογή της δημιουργίας προεπισκόπησης. |
|

**Returns:**
java.io.OutputStream - Μία παρουσία του java.io.OutputStream που περιέχει μια εικόνα της σελίδας του εγγράφου·  null  εάν η δημιουργία προεπισκόπησης σελίδας δεν υποστηρίζεται.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Λάβετε προεπισκόπηση σελίδων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Οι επιλογές για τον καθορισμό απαιτήσεων και αντιπροσώπων ροής για τη δημιουργία προεπισκόπησης. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Επιστρέφει τις γενικές πληροφορίες για το έγγραφο.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε πληροφορίες εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Get the document info
     IDocumentInfo info = parser.getDocumentInfo();
     // Print document information
     System.out.println(String.format("FileType: %s", info.getFileType()));
     System.out.println(String.format("PageCount: %d", info.getPageCount()));
     System.out.println(String.format("Size: %d", info.getSize()));
 }
 
````



**Returns:**
[IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) - An instance of class that implements [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) interface.

### getText() {#getText--}
```
public TextReader getText()
```


Εξάγει κείμενο από το έγγραφο.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε κείμενο από ένα έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a text into the reader
     try (TextReader reader = parser.getText()) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(TextOptions options) {#getText-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(TextOptions options)
```


Εξάγει μια σελίδα κειμένου από το έγγραφο χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε ακατέργαστο κείμενο από ένα έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a raw text into the reader
     try (TextReader reader = parser.getText(new TextOptions(true))) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Οι επιλογές εξαγωγής κειμένου. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Εξάγει κείμενο από τη σελίδα του εγγράφου.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε κείμενο από τη σελίδα του εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Check if the document supports text extraction
     if (!parser.getFeatures().isText()) {
         System.out.println("Document isn't supports text extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int p = 0; p < documentInfo.getPageCount(); p++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", p + 1, documentInfo.getPageCount()));
         // Extract a text into the reader
         try (TextReader reader = parser.getText(p)) {
             // Print a text from the document
             // We ignore null-checking as we have checked text extraction feature support earlier
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Εξάγει κείμενο από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές κειμένου (για ενεργοποίηση της ακατέργαστης γρήγορης λειτουργίας εξαγωγής κειμένου).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε ακατέργαστο κείμενο από τη σελίδα του εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Check if the document supports text extraction
     if (!parser.getFeatures().isText()) {
         System.out.println("Document isn't supports text extraction.");
         return;
     }
     // Get the document info
     DocumentInfo documentInfo = parser.getDocumentInfo() instanceof DocumentInfo
             ? (DocumentInfo) parser.getDocumentInfo()
             : null;
     // Check if the document has pages
     if (documentInfo == null || documentInfo.getRawPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int p = 0; p < documentInfo.getRawPageCount(); p++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", p + 1, documentInfo.getPageCount()));
         // Extract a text into the reader
         try (TextReader reader = parser.getText(p, new TextOptions(true))) {
             // Print a text from the document
             // We ignore null-checking as we have checked text extraction feature support earlier
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Οι επιλογές εξαγωγής κειμένου. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Εξάγει μορφοποιημένο κείμενο από το έγγραφο.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε το κείμενο του εγγράφου ως κείμενο HTML:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Extract a formatted text into the reader
     try (TextReader reader = parser.getFormattedText(new FormattedTextOptions(FormattedTextMode.Html))) {
         // Print a formatted text from the document
         // If formatted text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Formatted text extraction isn't suppported" : reader.readToEnd());
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Οι επιλογές εξαγωγής μορφοποιημένου κειμένου. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Εξάγει μορφοποιημένο κείμενο από τη σελίδα του εγγράφου.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε το κείμενο της σελίδας του εγγράφου ως κείμενο Markdown:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Check if the document supports formatted text extraction
     if (!parser.getFeatures().isFormattedText()) {
         System.out.println("Document isn't supports formatted text extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int p = 0; p < documentInfo.getPageCount(); p++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", p + 1, documentInfo.getPageCount()));
         // Extract a formatted text into the reader
         try (TextReader reader = parser.getFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown))) {
             // Print a formatted text from the document
             // We ignore null-checking as we have checked formatted text extraction feature support earlier
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Οι επιλογές εξαγωγής μορφοποιημένου κειμένου. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Αναζητά μια λέξη-κλειδί στο έγγραφο.

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

Το παρακάτω παράδειγμα δείχνει πώς να βρείτε μια λέξη-κλειδί σε ένα έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Search a keyword:
     Iterable sr = parser.search("lorem");
     // Check if search is supported
     if (sr == null) {
         System.out.println("Search isn't supported");
         return;
     }
     // Iterate over search results
     for (SearchResult s : sr) {
         // Print an index and found text:
         System.out.println(String.format("At %d: %s", s.getPosition(), s.getText()));
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη-κλειδί | java.lang.String | Η λέξη-κλειδί για αναζήτηση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Μια συλλογή αντικειμένων [SearchResult](../../com.groupdocs.parser.data/searchresult);  null  εάν η αναζήτηση δεν υποστηρίζεται.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Αναζητά μια λέξη-κλειδί στο έγγραφο χρησιμοποιώντας επιλογές αναζήτησης (κανονική έκφραση, ευαίσθητο σε πεζά/κεφαλαία, κ.λπ.).

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

Το παρακάτω παράδειγμα δείχνει πώς να αναζητήσετε με κανονική έκφραση σε ένα έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Search with a regular expression with case matching
     Iterable sr = parser.search("[0-9]+", new SearchOptions(true, false, true));
     // Check if search is supported
     if (sr == null) {
         System.out.println("Search isn't supported");
         return;
     }
     // Iterate over search results
     for (SearchResult s : sr) {
         // Print an index and found text:
         System.out.println(String.format("At %d: %s", s.getPosition(), s.getText()));
     }
 }
 
````

Το παρακάτω παράδειγμα δείχνει πώς να αναζητήσετε κείμενο σε σελίδες:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Search a keyword with page numbers
     Iterable sr = parser.search("lorem", new SearchOptions(false, false, false, true));
     // Check if search is supported
     if (sr == null) {
         System.out.println("Search isn't supported");
         return;
     }
     // Iterate over search results
     for (SearchResult s : sr) {
         // Print an index, page number and found text:
         System.out.println(String.format("At %d (%d): %s", s.getPosition(), s.getPageIndex(), s.getText()));
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | λέξη-κλειδί | java.lang.String | Η λέξη-κλειδί για αναζήτηση. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Οι επιλογές αναζήτησης. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Μια συλλογή αντικειμένων [SearchResult](../../com.groupdocs.parser.data/searchresult);  null  εάν η αναζήτηση δεν υποστηρίζεται.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Εξάγει επισήμανση από το έγγραφο.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε μια επισήμανση που περιέχει 3 λέξεις:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a highlight:
     HighlightItem hl = parser.getHighlight(2, true, new HighlightOptions(10, 3));
     // Check if highlight extraction is supported
     if (hl == null) {
         System.out.println("Highlight extraction isn't supported");
         return;
     }
     // Print an extracted highlight
     System.out.println(String.format("At %d: %s", hl.getPosition(), hl.getText()));
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | θέση | int | Η αρχική θέση της επισήμανσης. |
|
|  | isDirect | boolean | Η τιμή που υποδεικνύει εάν η εξαγωγή επισήμανσης είναι άμεση.  true  αν η επισήμανση εξάγεται από τη δεξιά πλευρά της θέσης· διαφορετικά,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές εξαγωγής επισήμανσης. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Εξάγει πίνακα περιεχομένων από το έγγραφο.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε τον πίνακα περιεχομένων από αρχείο EPUB:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleEpub)) {
     // Check if text extraction is supported
     if (!parser.getFeatures().isText()) {
         System.out.println("Text extraction isn't supported.");
         return;
     }
     // Check if toc extraction is supported
     if (!parser.getFeatures().isToc()) {
         System.out.println("Toc extraction isn't supported.");
         return;
     }
     // Get table of contents
     Iterable toc = parser.getToc();
     // Iterate over items
     for (TocItem i : toc) {
         // Print the Toc text
         System.out.println(i.getText());
         // Check if page index has a value
         if (i.getPageIndex() == null) {
             continue;
         }
         // Extract a page text
         try (TextReader reader = parser.getText(i.getPageIndex())) {
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - Μια συλλογή στοιχείων πίνακα περιεχομένων·  null  εάν η εξαγωγή πίνακα περιεχομένων δεν υποστηρίζεται.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Εξάγει μεταδεδομένα από το έγγραφο.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε μεταδεδομένα από ένα έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Extract metadata from the document
     Iterable metadata = parser.getMetadata();
     // Check if metadata extraction is supported
     if (metadata == null) {
         System.out.println("Metatada extraction isn't supported");
     }
     // Iterate over metadata items
     for (MetadataItem item : metadata) {
         // Print an item name and value
         System.out.println(String.format("%s: %s", item.getName(), item.getValue()));
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Μια συλλογή στοιχείων μεταδεδομένων·  null  εάν η εξαγωγή μεταδεδομένων δεν υποστηρίζεται.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Εξάγει σχολιασμούς από το έγγραφο.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Μια συλλογή στοιχείων σχολιασμού·  null  εάν η εξαγωγή σχολιασμού δεν υποστηρίζεται.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Εξάγει σχολιασμούς από τη σελίδα του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Μια συλλογή στοιχείων σχολιασμού·  null  εάν η εξαγωγή σχολιασμού δεν υποστηρίζεται.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Εξάγει ένα αντικείμενο container από το έγγραφο για εργασία με μορφές που περιέχουν συνημμένα, αρχεία ZIP κ.ά.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε κείμενο από οντότητες zip:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over zip entities
     for (ContainerItem item : attachments) {
         // Print the file path
         System.out.println(item.getFilePath());
         try {
             // Create Parser object for the zip entity content
             try (Parser attachmentParser = item.openParser()) {
                 // Extract an zip entity text
                 try (TextReader reader = attachmentParser.getText()) {
                     System.out.println(reader == null ? "No text" : reader.readToEnd());
                 }
             }
         } catch (UnsupportedDocumentFormatException ex) {
             System.out.println("Isn't supported.");
         }
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Μια συλλογή στοιχείων κοντέινερ·  null  εάν η εξαγωγή κοντέινερ δεν υποστηρίζεται.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Εξάγει περιοχές κειμένου από το έγγραφο.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις περιοχές κειμένου από ολόκληρο το έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Extract text areas
     Iterable areas = parser.getTextAreas();
     // Check if text areas extraction is supported
     if (areas == null) {
         System.out.println("Page text areas extraction isn't supported");
         return;
     }
     // Iterate over page text areas
     for (PageTextArea a : areas) {
         // Print a page index, rectangle and text area value:
         System.out.println(String.format("Page: %d, R: %s, Text: %s", a.getPage().getIndex(), a.getRectangle(), a.getText()));
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Μια συλλογή αντικειμένων [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Εξάγει περιοχές κειμένου από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, ταίριασμα πεζών/κεφαλαίων, κ.λπ.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε μόνο περιοχές κειμένου με ψηφία από την πάνω αριστερή γωνία:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Create the options which are used for text area extraction
     PageTextAreaOptions options = new PageTextAreaOptions("\\s[a-z]{2}\\s", new Rectangle(new Point(0, 0), new Size(300, 100)));
     // Extract text areas which contain only digits from the upper-left corner of a page:
     Iterable areas = parser.getTextAreas(options);
     // Check if text areas extraction is supported
     if (areas == null) {
         System.out.println("Page text areas extraction isn't supported");
         return;
     }
     // Iterate over page text areas
     for (PageTextArea a : areas) {
         // Print a page index, rectangle and text area value:
         System.out.println(String.format("Page: %d, R: %s, Text: %s", a.getPage().getIndex(), a.getRectangle(), a.getText()));
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Οι επιλογές για εξαγωγή περιοχών κειμένου. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Μια συλλογή αντικειμένων [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Για την εξαγωγή περιοχών κειμένου από μια σελίδα εγγράφου χρησιμοποιείται η παρακάτω μέθοδος:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Check if the document supports text areas extraction
     if (!parser.getFeatures().isTextAreas()) {
         System.out.println("Document isn't supports text areas extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Iterate over page text areas
         // We ignore null-checking as we have checked text areas extraction feature support earlier
         for (PageTextArea a : parser.getTextAreas(pageIndex)) {
             // Print a rectangle and text area value:
             System.out.println(String.format("R: %s, Text: %s", a.getRectangle(), a.getText()));
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Μια συλλογή αντικειμένων [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Εξάγει περιοχές κειμένου από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (κανονική έκφραση, ταίριασμα πεζών/κεφαλαίων, κ.λπ.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Οι επιλογές για εξαγωγή περιοχών κειμένου. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Μια συλλογή αντικειμένων [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  εάν η εξαγωγή περιοχών κειμένου δεν υποστηρίζεται.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Εξάγει εικόνες από το έγγραφο.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλες τις εικόνες από ολόκληρο το έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Extract images
     Iterable images = parser.getImages();
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Images extraction isn't supported");
         return;
     }
     // Iterate over images
     for (PageImageArea image : images) {
         // Print a page index, rectangle and image type:
         System.out.println(String.format("Page: %d, R: %s, Type: %s", image.getPage().getIndex(), image.getRectangle(), image.getFileType()));
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Μια συλλογή αντικειμένων [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Εξάγει εικόνες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει εικόνες).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε μόνο εικόνες από την πάνω αριστερή γωνία:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Create the options which are used for images extraction
     PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(340, 150), new Size(300, 100)));
     // Extract images from the upper-left corner of a page:
     Iterable images = parser.getImages(options);
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }
     // Iterate over images
     for (PageImageArea image : images) {
         // Print a page index, rectangle and image type:
         System.out.println(String.format("Page: %d, R: %s, Type: %s", image.getPage().getIndex(), image.getRectangle(), image.getFileType()));
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Οι επιλογές για εξαγωγή εικόνων. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Μια συλλογή αντικειμένων [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Εξάγει εικόνες από τη σελίδα του εγγράφου.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Για την εξαγωγή εικόνων από μια σελίδα εγγράφου χρησιμοποιείται η παρακάτω μέθοδος:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleImagesPdf)) {
     // Check if the document supports images extraction
     if (!parser.getFeatures().isImages()) {
         System.out.println("Document isn't supports images extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Iterate over images
         // We ignore null-checking as we have checked images extraction feature support earlier
         for (PageImageArea image : parser.getImages(pageIndex)) {
             // Print a rectangle and image type
             System.out.println(String.format("R: %s, Text: %s", image.getRectangle(), image.getFileType()));
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Μια συλλογή αντικειμένων [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Εξάγει εικόνες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει εικόνες).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Οι επιλογές για εξαγωγή εικόνων. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Μια συλλογή αντικειμένων [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  εάν η εξαγωγή εικόνων δεν υποστηρίζεται.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Εξάγει υπερσυνδέσμους από το έγγραφο.

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε όλους τους υπερσυνδέσμους από ολόκληρο το έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Extract hyperlinks from the document
     Iterable hyperlinks = parser.getHyperlinks();
     // Iterate over hyperlinks
     for (PageHyperlinkArea h : hyperlinks) {
         // Print the hyperlink text
         System.out.println(h.getText());
         // Print the hyperlink URL
         System.out.println(h.getUrl());
         System.out.println();
     }
 }
 
````



**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Μια συλλογή αντικειμένων [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου.

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε υπερσυνδέσμους από τη σελίδα του εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Extract hyperlinks from the document page
         Iterable hyperlinks = parser.getHyperlinks(pageIndex);
         // Iterate over hyperlinks
         for (PageHyperlinkArea h : hyperlinks) {
             // Print the hyperlink text
             System.out.println(h.getText());
             // Print the hyperlink URL
             System.out.println(h.getUrl());
             System.out.println();
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Μια συλλογή αντικειμένων [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Εξάγει υπερσυνδέσμους από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει υπερσυνδέσμους).

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε υπερσυνδέσμους από την περιοχή της σελίδας του εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.HyperlinksPdf)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Create the options which are used for hyperlink extraction
     PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
     // Extract hyperlinks from the document page area
     Iterable hyperlinks = parser.getHyperlinks(options);
     // Iterate over hyperlinks
     for (PageHyperlinkArea h : hyperlinks) {
         // Print the hyperlink text
         System.out.println(h.getText());
         // Print the hyperlink URL
         System.out.println(h.getUrl());
         System.out.println();
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Οι επιλογές για εξαγωγή υπερσυνδέσμων. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Μια συλλογή αντικειμένων [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Εξάγει υπερσυνδέσμους από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει υπερσυνδέσμους).

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε υπερσυνδέσμους από την περιοχή σελίδας του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports hyperlink extraction
     if (!parser.getFeatures().isHyperlinks()) {
         System.out.println("Document isn't supports hyperlink extraction.");
         return;
     }
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Create the options which are used for hyperlink extraction
     PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Extract hyperlinks from the document page
         Iterable hyperlinks = parser.getHyperlinks(pageIndex, options);
         // Iterate over hyperlinks
         for (PageHyperlinkArea h : hyperlinks) {
             // Print the hyperlink text
             System.out.println(h.getText());
             // Print the hyperlink URL
             System.out.println(h.getUrl());
             System.out.println();
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Οι επιλογές για εξαγωγή υπερσυνδέσμων. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Μια συλλογή αντικειμένων [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  εάν η εξαγωγή υπερσυνδέσμων δεν υποστηρίζεται.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Εξάγει γραμμωτούς κώδικες από το έγγραφο.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Μια συλλογή από αντικείμενα [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  εάν η εξαγωγή barcode δεν υποστηρίζεται.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Εξάγει γραμμωτούς κώδικες από τη σελίδα του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Μια συλλογή από αντικείμενα [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  εάν η εξαγωγή barcode δεν υποστηρίζεται.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Εξάγει γραμμωτούς κώδικες από το έγγραφο χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει γραμμωτούς κώδικες).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Οι επιλογές για την εξαγωγή barcode. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Μια συλλογή από αντικείμενα [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  εάν η εξαγωγή barcode δεν υποστηρίζεται.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Εξάγει γραμμωτούς κώδικες από τη σελίδα του εγγράφου χρησιμοποιώντας επιλογές προσαρμογής (για ορισμό του ορθογωνίου περιοχής που περιέχει γραμμωτούς κώδικες).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Οι επιλογές για την εξαγωγή barcode. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Μια συλλογή από αντικείμενα [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  εάν η εξαγωγή barcode δεν υποστηρίζεται.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Εξάγει πίνακες από το έγγραφο.

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε πίνακες από ολόκληρο το έγγραφο:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Check if the document supports table extraction
     if (!parser.getFeatures().isTables()) {
         System.out.println("Document isn't supports tables extraction.");
         return;
     }
     // Create the layout of tables
     TemplateTableLayout layout = new TemplateTableLayout(
             java.util.Arrays.asList(new Double[]{50.0, 95.0, 275.0, 415.0, 485.0, 545.0}),
             java.util.Arrays.asList(new Double[]{325.0, 340.0, 365.0, 395.0}));
     // Create the options for table extraction
     PageTableAreaOptions options = new PageTableAreaOptions(layout);
     // Extract tables from the document
     Iterable tables = parser.getTables(options);
     // Iterate over tables
     for (PageTableArea t : tables) {
         // Iterate over rows
         for (int row = 0; row < t.getRowCount(); row++) {
             // Iterate over columns
             for (int column = 0; column < t.getColumnCount(); column++) {
                 // Get the table cell
                 PageTableAreaCell cell = t.getCell(row, column);
                 if (cell != null) {
                     // Print the table cell text
                     System.out.print(cell.getText());
                     System.out.print(" | ");
                 }
             }
             System.out.println();
         }
         System.out.println();
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Οι επιλογές για την εξαγωγή πινάκων. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Μια συλλογή από αντικείμενα [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Εξάγει πίνακες από το έγγραφο, εντοπίζοντάς τους αυτόματα.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Μια συλλογή από αντικείμενα [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Εξάγει πίνακες από τη σελίδα του εγγράφου.

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε πίνακες από τη σελίδα του εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleInvoicePagesPdf)) {
     // Check if the document supports table extraction
     if (!parser.getFeatures().isTables()) {
         System.out.println("Document isn't supports tables extraction.");
         return;
     }
     // Create the layout of tables
     TemplateTableLayout layout = new TemplateTableLayout(
             java.util.Arrays.asList(new Double[]{50.0, 95.0, 275.0, 415.0, 485.0, 545.0}),
             java.util.Arrays.asList(new Double[]{325.0, 340.0, 365.0, 395.0}));
     // Create the options for table extraction
     PageTableAreaOptions options = new PageTableAreaOptions(layout);
     // Get the document info
     IDocumentInfo documentInfo = parser.getDocumentInfo();
     // Check if the document has pages
     if (documentInfo.getPageCount() == 0) {
         System.out.println("Document hasn't pages.");
         return;
     }
     // Iterate over pages
     for (int pageIndex = 0; pageIndex < documentInfo.getPageCount(); pageIndex++) {
         // Print a page number
         System.out.println(String.format("Page %d/%d", pageIndex + 1, documentInfo.getPageCount()));
         // Extract tables from the document page
         Iterable tables = parser.getTables(pageIndex, options);
         // Iterate over tables
         for (PageTableArea t : tables) {
             // Iterate over rows
             for (int row = 0; row < t.getRowCount(); row++) {
                 // Iterate over columns
                 for (int column = 0; column < t.getColumnCount(); column++) {
                     // Get the table cell
                     PageTableAreaCell cell = t.getCell(row, column);
                     if (cell != null) {
                         // Print the table cell text
                         System.out.print(cell.getText());
                         System.out.print(" | ");
                     }
                 }
                 System.out.println();
             }
             System.out.println();
         }
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Οι επιλογές για την εξαγωγή πινάκων. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Μια συλλογή από αντικείμενα [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Εξάγει πίνακες από τη σελίδα του εγγράφου, εντοπίζοντάς τους αυτόματα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Μια συλλογή από αντικείμενα [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  εάν η εξαγωγή πινάκων δεν υποστηρίζεται.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Δημιουργεί μια συλλογή προσαρμογών [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s για το έγγραφο.

Αντίγραφο Java της C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (υποβολές d4e691b /
ae9e98c). Χρήσιμο ως πρότυπο εκκίνησης που ο χρήστης μπορεί στη συνέχεια να περικόψει ή να μετονομάσει.

### Algorithm

1. Επιλέξτε τη σελίδα από  options.getPageIndex()  (προεπιλογή  0 ).
2. Εάν το έγγραφο υποστηρίζει εξαγωγή περιοχών κειμένου, καλέστε #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) και δημιουργήστε ένα [TemplateField](../../com.groupdocs.parser.templates/templatefield) ανά μη κενή περιοχή κειμένου, με όνομα  {prefix}_{n}  (προεπιλεγμένο πρόθεμα  "Field" ). Κάθε πεδίο λαμβάνει ένα [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) στο ορθογώνιο της περιοχής κειμένου, με το πλάτος της σελίδας καταγεγραμμένο ως  pageWidth  ώστε η επακόλουθη κλιμάκωση του προτύπου να λειτουργεί.
3. Εάν το έγγραφο δεν υποστηρίζει περιοχές κειμένου, επιστρέψτε  null .

### OCR caveat

Η υλοποίηση C# εκτελεί OCR πάνω στην προεπισκόπηση της σελίδας για να δημιουργήσει πεδία όταν το έγγραφο είναι μόνο εικόνα. Το [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) της Java παρέχεται από τον χρήστη, έτσι η δημιουργία με βάση το OCR είναι σημαντική μόνο εάν έχει ρυθμιστεί ένας σύνδεσμος ΚΑΙ η μέθοδος recognizeTextAreas(...) του συνδέσμου επιστρέφει σωστά ορθογώνια. Όταν το  options.getOcrOptions()  είναι ορισμένο και υπάρχει σύνδεσμος, προτιμάται η διαδικασία OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Οι επιλογές δημιουργίας. Μπορεί να είναι  null  (εφαρμόζονται προεπιλογές). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Ένα iterable από παραγόμενα [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s, ή  null  εάν δεν υποστηρίζεται από αυτή τη μορφή εγγράφου.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Εξάγει τις πληροφορίες για όλα τα φύλλα εργασίας στο λογιστικό φύλλο.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Μια λίστα από αντικείμενα [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) που περιέχουν πληροφορίες για όλα τα φύλλα εργασίας στο λογιστικό φύλλο.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Εξάγει τις πληροφορίες για το φύλλο εργασίας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | worksheetIndex | int | Ο δείκτης μηδενικής βάσης του φύλλου εργασίας. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Εξάγει κελιά του φύλλου εργασίας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | worksheetIndex | int | Ο δείκτης μηδενικής βάσης του φύλλου εργασίας. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Μια συλλογή από αντικείμενα [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) που περιέχουν τα δεδομένα του κελιού.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Εξάγει κελιά του φύλλου εργασίας χρησιμοποιώντας επιλογές προσαρμογής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | worksheetIndex | int | Ο δείκτης μηδενικής βάσης του φύλλου εργασίας. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Οι επιλογές εξαγωγής φύλλου εργασίας. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Μια συλλογή από αντικείμενα [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) που περιέχουν τα δεδομένα του κελιού.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Αναλύει το έγγραφο με το πρότυπο που δημιουργήθηκε από τον χρήστη.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Το πρότυπο που δημιουργήθηκε από τον χρήστη. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Αναλύει το έγγραφο με το πρότυπο που δημιουργήθηκε από τον χρήστη, με τις παρεχόμενες επιλογές.

Εάν
options.getPageIndex()
είναι ορισμένο, μόνο αυτή η σελίδα αναλύεται· διαφορετικά όλες οι σελίδες αναλύονται.

Η υποστήριξη OCR εξαρτάται από το [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) που έχει ρυθμιστεί στο [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Το πρότυπο που δημιουργήθηκε από τον χρήστη. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Οι επιλογές ανάλυσης κατά πρότυπο. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Αναλύει το έγγραφο επιλέγοντας αυτόματα το πιο κατάλληλο πρότυπο από μια συλλογή.

Αντίγραφο του C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
εισήχθη στο commit 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), και το πρότυπο που αποδίδει
κερδίζει ο αριθμός με τις περισσότερες συμπληρωμένες πεδία (μη-μηδενικές περιοχές σελίδας με μη-κενό κείμενο). Η υλοποίηση C# χρησιμοποιεί
η αντιστοίχιση hidden-marker κατά τη διάρκεια μιας διεργασίας OCR· αυτή η διαδρομή δεν είναι ακόμη διαθέσιμη στη Java επειδή οι δείκτες hidden-field και
ο TemplatePageOcrParser που βασίζεται σε OCR δεν έχουν μεταφερθεί, έτσι αυτός ο αριθμός συμπληρωμένων πεδίων χρησιμοποιείται ως διαφανής εναλλακτική λύση.
Οι κλήσεις που χρειάζονται συμπεριφορά παρόμοια με τη C# θα πρέπει να ενσωματώσουν έναν προσαρμοσμένο επιλογέα μόλις η μηχανή OCR είναι συνδεδεμένη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Μια συλλογή υποψήφιων προτύπων. Ο αναλυτής θα επιλέξει το πιο κατάλληλο. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Επιλογές ανάλυσης. Μπορεί να είναι  null . |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Αναλύει τη φόρμα του εγγράφου.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Το παρακάτω παράδειγμα δείχνει πώς να αναλύσετε μια μορφή του εγγράφου:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### getStructure() {#getStructure--}
```
public Document getStructure()
```


Εξάγει δομημένο κείμενο από το έγγραφο.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - Μία παρουσία της κλάσης  org.w3c.dom.Document  με δομή κειμένου XML·  null  εάν η εξαγωγή δομής κειμένου δεν υποστηρίζεται.

### close() {#close--}
```
public void close()
```


Κλείνει αυτόν τον πόρο, απελευθερώνοντας τυχόν υποκείμενους πόρους.


