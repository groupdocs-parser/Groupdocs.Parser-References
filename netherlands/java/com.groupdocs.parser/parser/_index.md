---
title: "Parser"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de hoofdklasse voor die de extractie van tekst‑ en afbeeldingscontainers en de parseerfunctionaliteit beheert."
type: docs
weight: 10
url: /nl/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Stelt de hoofdklasse voor die de functionaliteit voor tekst, afbeeldingen, container-extractie en parsing regelt.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren met  loadOptions . |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren met  parserSettings . |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren met  loadOptions  en  parserSettings . |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens uit een database te extraheren. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens uit een database te extraheren. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse. |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse. |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse. |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions) en [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse. |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions) en [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Geeft de algemene informatie over een bestand terug. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Geeft de algemene informatie over een bestand terug. |
|
|  | [getFeatures()](#getFeatures--) | Haalt de ondersteunde functies op. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Genereert een voorbeeld van een documentpagina. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Genereert een voorbeeld van een documentpagina met behulp van aanpassingsopties. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Haal voorbeeld van pagina's op. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Geeft de algemene informatie over het document terug. |
|
|  | [getText()](#getText--) | Extraheert tekst uit het document. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Extraheert een tekstpagina uit het document met behulp van tekstopties (om de ruwe snelle teksteextractiemodus in te schakelen). |
|
|  | [getText(int pageIndex)](#getText-int-) | Extraheert tekst uit de documentpagina. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Extraheert tekst uit de documentpagina met behulp van tekstopties (om de ruwe snelle teksteextractiemodus in te schakelen). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Extraheert opgemaakte tekst uit het document. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Extraheert opgemaakte tekst uit de documentpagina. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Zoekt een trefwoord in het document. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Zoekt een trefwoord in het document met behulp van zoekopties (reguliere expressie, hoofdlettergevoelig, enz.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Extraheert een markering uit het document. |
|
|  | [getToc()](#getToc--) | Extraheert een inhoudsopgave uit het document. |
|
|  | [getMetadata()](#getMetadata--) | Extraheert metadata uit het document. |
|
|  | [getAnnotations()](#getAnnotations--) | Extraheert annotaties uit het document. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Extraheert annotaties uit de documentpagina. |
|
|  | [getContainer()](#getContainer--) | Extraheert een containerobject uit het document om te werken met formaten die bijlagen, ZIP-archieven enz. bevatten. |
|
|  | [getTextAreas()](#getTextAreas--) | Extraheert tekstgebieden uit het document. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Extraheert tekstgebieden uit het document met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoelig zoeken, enz.). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Extraheert tekstgebieden uit de documentpagina. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Extraheert tekstgebieden uit de documentpagina met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoelig zoeken, enz.). |
|
|  | [getImages()](#getImages--) | Extraheert afbeeldingen uit het document. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Extraheert afbeeldingen uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Extraheert afbeeldingen uit de documentpagina. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Extraheert afbeeldingen uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Extraheert hyperlinks uit het document. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Extraheert hyperlinks uit de documentpagina. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Extraheert hyperlinks uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Extraheert hyperlinks uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen). |
|
|  | [getBarcodes()](#getBarcodes--) | Extraheert barcodes uit het document. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Extraheert barcodes uit de documentpagina. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Extraheert barcodes uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat barcodes bevat in te stellen). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Extraheert barcodes uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat barcodes bevat in te stellen). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Extraheert tabellen uit het document. |
|
|  | [getTables()](#getTables--) | Extraheert tabellen uit het document, waarbij ze automatisch worden gedetecteerd. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Extraheert tabellen uit de documentpagina. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Extraheert tabellen uit de documentpagina, waarbij ze automatisch worden gedetecteerd. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Genereert een verzameling aanpassings-[TemplateItem](../../com.groupdocs.parser.templates/templateitem)s voor het document. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Extraheert de informatie over alle werkbladen in de spreadsheet. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Extraheert de informatie over het werkblad. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Extraheert werkbladcellen. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Extraheert werkbladcellen met behulp van aanpassingsopties. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Parseert het document met het door de gebruiker gegenereerde sjabloon. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Parseert het document met het door de gebruiker gegenereerde sjabloon met de meegeleverde opties. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Parseert het document door automatisch de best passende sjabloon uit een collectie te selecteren. |
|
|  | [parseForm()](#parseForm--) | Parseert het documentformulier. |
|
|  | [getStructure()](#getStructure--) | Extraheert gestructureerde tekst uit het document. |
|
|  | [close()](#close--) | Sluit deze bron en geeft alle onderliggende bronnen vrij. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | url | java.net.URL | De URL waar het verzoek naartoe wordt gestuurd |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren met  loadOptions .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | url | java.net.URL | De URL waar het verzoek naartoe wordt gestuurd. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om het bestand te openen. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren met  parserSettings .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | url | java.net.URL | De URL waar het verzoek naartoe wordt gestuurd. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens van een URL te extraheren met  loadOptions  en  parserSettings .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | url | java.net.URL | De URL waar het verzoek naartoe wordt gestuurd. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om het bestand te openen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens uit een database te extraheren.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Het volgende voorbeeld toont hoe gegevens uit een Sqlite-database te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | verbinding | java.sql.Connection | De databaseverbinding. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse om gegevens uit een database te extraheren.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Het volgende voorbeeld toont hoe gegevens uit een Sqlite-database te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | verbinding | java.sql.Connection | De databaseverbinding. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Het volgende voorbeeld toont hoe e‑mails van Exchange Server te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | De e‑mailverbinding. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Het volgende voorbeeld toont hoe e‑mails van Exchange Server te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | De e‑mailverbinding. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Het volgende voorbeeld toont hoe het document van de lokale schijf te laden:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Het documentwachtwoord wordt door de klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) doorgegeven:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om het bestand te openen. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions) en [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Het volgende voorbeeld toont hoe de informatie via de interface [ILogger](../../com.groupdocs.parser.options/ilogger) te ontvangen:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om het bestand te openen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Het volgende voorbeeld toont hoe het document uit de stream te laden:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | De bron‑invoerstroom. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

In sommige gevallen is het nodig om [FileFormat](../../com.groupdocs.parser.options/fileformat) te definiëren. Zowel voor speciale gevallen (databases, e‑mailserver)
en voor het detecteren van bestandstypen op basis van de inhoud:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | De bron‑invoerstroom. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om het bestand te openen. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | De bron‑invoerstroom. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initialiseert een nieuw exemplaar van de [Parser](../../com.groupdocs.parser/parser) klasse met [LoadOptions](../../com.groupdocs.parser.options/loadoptions) en [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Het volgende voorbeeld toont hoe de informatie via de interface [ILogger](../../com.groupdocs.parser.options/ilogger) te ontvangen:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | De bron‑invoerstroom. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om het bestand te openen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Geeft de algemene informatie over een bestand terug.

De volgende code toont hoe te controleren of een bestand met een wachtwoord is beveiligd:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Geeft de algemene informatie over een bestand terug.

De volgende code toont hoe te controleren of een bestand met een wachtwoord is beveiligd:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | De bron‑invoerstroom. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Haalt de ondersteunde functies op.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Als de functie niet wordt ondersteund, retourneert de methode
null
in plaats van de waarde. Sommige bewerkingen kunnen verbruiken
aanzienlijke tijd. Dus is het niet optimaal om de methode aan te roepen alleen om de ondersteuning van de functie te controleren.
Voor dit doel wordt de eigenschap Features gebruikt:

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


Genereert een voorbeeld van een documentpagina.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.io.OutputStream - Een instantie van java.io.OutputStream die een afbeelding van de documentpagina bevat;  null  als het genereren van een paginavoorbeeld niet wordt ondersteund.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Genereert een voorbeeld van een documentpagina met behulp van aanpassingsopties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | De opties om de generatie van het voorbeeld aan te passen. |
|

**Returns:**
java.io.OutputStream - Een instantie van java.io.OutputStream die een afbeelding van de documentpagina bevat;  null  als het genereren van een paginavoorbeeld niet wordt ondersteund.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Haal voorbeeld van pagina's op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | De opties om vereisten en streamdelegaten in te stellen voor de generatie van het voorbeeld. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Geeft de algemene informatie over het document terug.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Het volgende voorbeeld toont hoe documentinformatie op te halen:

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


Extraheert tekst uit het document.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Het volgende voorbeeld toont hoe tekst uit een document te extraheren:

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


Extraheert een tekstpagina uit het document met behulp van tekstopties (om de ruwe snelle teksteextractiemodus in te schakelen).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Het volgende voorbeeld toont hoe ruwe tekst uit een document te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | De opties voor tekstelextractie. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Extraheert tekst uit de documentpagina.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Het volgende voorbeeld toont hoe tekst van de documentpagina te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Extraheert tekst uit de documentpagina met behulp van tekstopties (om de ruwe snelle teksteextractiemodus in te schakelen).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Het volgende voorbeeld toont hoe ruwe tekst van de documentpagina te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | De opties voor tekstelextractie. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Extraheert opgemaakte tekst uit het document.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Het volgende voorbeeld toont hoe documenttekst als HTML-tekst te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | De opties voor geformatteerde tekstelextractie. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Extraheert opgemaakte tekst uit de documentpagina.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Het volgende voorbeeld toont hoe documentpaginatekst als Markdown-tekst te extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | De opties voor geformatteerde tekstelextractie. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Zoekt een trefwoord in het document.

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

Het volgende voorbeeld toont hoe een trefwoord in een document te vinden:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | trefwoord | java.lang.String | Het trefwoord om te zoeken. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Een collectie van [SearchResult](../../com.groupdocs.parser.data/searchresult) objecten;  null  als zoeken niet wordt ondersteund.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Zoekt een trefwoord in het document met behulp van zoekopties (reguliere expressie, hoofdlettergevoelig, enz.).

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

Het volgende voorbeeld toont hoe met een reguliere expressie in een document te zoeken:

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

Het volgende voorbeeld toont hoe tekst op pagina's te zoeken:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | trefwoord | java.lang.String | Het trefwoord om te zoeken. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | De zoekopties. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Een collectie van [SearchResult](../../com.groupdocs.parser.data/searchresult) objecten;  null  als zoeken niet wordt ondersteund.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Extraheert een markering uit het document.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Het volgende voorbeeld toont hoe een markering te extraheren die 3 woorden bevat:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | positie | int | De startpositie van de markering. |
|
|  | isDirect | boolean | De waarde die aangeeft of highlight-extractie direct is.  true  als de higlight wordt geëxtraheerd vanaf de rechterkant van de positie; anders,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De highlight-extractie-opties. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Extraheert een inhoudsopgave uit het document.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Het volgende voorbeeld toont hoe je de inhoudsopgave uit een EPUB-bestand kunt extraheren:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - Een collectie van inhoudsopgave-items;  null  als inhoudsopgave-extractie niet wordt ondersteund.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Extraheert metadata uit het document.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Het volgende voorbeeld toont hoe je metadata uit een document kunt extraheren:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Een collectie van metadata-items;  null  als metadata-extractie niet wordt ondersteund.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Extraheert annotaties uit het document.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Een collectie van annotatie-items;  null  als annotatie-extractie niet wordt ondersteund.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Extraheert annotaties uit de documentpagina.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Een collectie van annotatie-items;  null  als annotatie-extractie niet wordt ondersteund.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Extraheert een containerobject uit het document om te werken met formaten die bijlagen, ZIP-archieven enz. bevatten.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Het volgende voorbeeld toont hoe je tekst uit zip-entiteiten kunt extraheren:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Een collectie van container-items;  null  als container-extractie niet wordt ondersteund.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Extraheert tekstgebieden uit het document.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Het volgende voorbeeld toont hoe je alle tekstgebieden uit het volledige document kunt extraheren:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Een collectie van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objecten;  null  als extractie van tekstgebieden niet wordt ondersteund.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Extraheert tekstgebieden uit het document met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoelig zoeken, enz.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Het volgende voorbeeld toont hoe je alleen tekstgebieden met cijfers uit de linkerbovenhoek kunt extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | De opties voor extractie van tekstgebieden. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Een collectie van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objecten;  null  als extractie van tekstgebieden niet wordt ondersteund.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Extraheert tekstgebieden uit de documentpagina.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Om tekstgebieden uit een documentpagina te extraheren, wordt de volgende methode gebruikt:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Een collectie van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objecten;  null  als extractie van tekstgebieden niet wordt ondersteund.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Extraheert tekstgebieden uit de documentpagina met behulp van aanpassingsopties (reguliere expressie, hoofdlettergevoelig zoeken, enz.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | De opties voor extractie van tekstgebieden. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Een collectie van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objecten;  null  als extractie van tekstgebieden niet wordt ondersteund.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Extraheert afbeeldingen uit het document.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Het volgende voorbeeld toont hoe je alle afbeeldingen uit het volledige document kunt extraheren:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Een collectie van [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objecten;  null  als afbeeldingsextractie niet wordt ondersteund.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Extraheert afbeeldingen uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Het volgende voorbeeld toont hoe je alleen afbeeldingen uit de linkerbovenhoek kunt extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | De opties voor afbeeldingsextractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Een collectie van [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objecten;  null  als afbeeldingsextractie niet wordt ondersteund.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Extraheert afbeeldingen uit de documentpagina.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Om afbeeldingen uit een documentpagina te extraheren, wordt de volgende methode gebruikt:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Een collectie van [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objecten;  null  als afbeeldingsextractie niet wordt ondersteund.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Extraheert afbeeldingen uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat afbeeldingen bevat in te stellen).

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | De opties voor afbeeldingsextractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Een collectie van [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objecten;  null  als afbeeldingsextractie niet wordt ondersteund.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Extraheert hyperlinks uit het document.

Het volgende voorbeeld toont hoe je alle hyperlinks uit het volledige document kunt extraheren:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Een collectie van [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objecten;  null  als hyperlink-extractie niet wordt ondersteund.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Extraheert hyperlinks uit de documentpagina.

Het volgende voorbeeld toont hoe je hyperlinks uit de documentpagina kunt extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Een collectie van [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objecten;  null  als hyperlink-extractie niet wordt ondersteund.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Extraheert hyperlinks uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen).

Het volgende voorbeeld toont hoe je hyperlinks uit het gebied van de documentpagina kunt extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | De opties voor hyperlink-extractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Een collectie van [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objecten;  null  als hyperlink-extractie niet wordt ondersteund.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Extraheert hyperlinks uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat hyperlinks bevat in te stellen).

Het volgende voorbeeld toont hoe u hyperlinks uit het paginagedeelte van het document kunt extraheren met behulp van aanpassingsopties:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | De opties voor hyperlink-extractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Een collectie van [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objecten;  null  als hyperlink-extractie niet wordt ondersteund.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Extraheert barcodes uit het document.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Een verzameling van [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objecten;  null  als barcode-extractie niet wordt ondersteund.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Extraheert barcodes uit de documentpagina.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Een verzameling van [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objecten;  null  als barcode-extractie niet wordt ondersteund.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Extraheert barcodes uit het document met behulp van aanpassingsopties (om het rechthoekige gebied dat barcodes bevat in te stellen).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | De opties voor barcode-extractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Een verzameling van [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objecten;  null  als barcode-extractie niet wordt ondersteund.\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Extraheert barcodes uit de documentpagina met behulp van aanpassingsopties (om het rechthoekige gebied dat barcodes bevat in te stellen).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | De opties voor barcode-extractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Een verzameling van [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objecten;  null  als barcode-extractie niet wordt ondersteund.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Extraheert tabellen uit het document.

Het volgende voorbeeld toont hoe u tabellen uit het volledige document kunt extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | De opties voor tabel-extractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Een verzameling van [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objecten;  null  als tabel-extractie niet wordt ondersteund.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Extraheert tabellen uit het document, waarbij ze automatisch worden gedetecteerd.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Een verzameling van [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objecten;  null  als tabel-extractie niet wordt ondersteund.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Extraheert tabellen uit de documentpagina.

Het volgende voorbeeld toont hoe u tabellen uit de documentpagina kunt extraheren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | De opties voor tabel-extractie. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Een verzameling van [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objecten;  null  als tabel-extractie niet wordt ondersteund.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Extraheert tabellen uit de documentpagina, waarbij ze automatisch worden gedetecteerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Een verzameling van [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objecten;  null  als tabel-extractie niet wordt ondersteund.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Genereert een verzameling aanpassings-[TemplateItem](../../com.groupdocs.parser.templates/templateitem)s voor het document.

Java-spiegel van de C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (commits d4e691b /
ae9e98c). Handig als een starttemplate die de gebruiker vervolgens kan inkorten of hernoemen.

### Algorithm

1. Kies de pagina uit  options.getPageIndex()  (standaard  0 ).
2. Als het document tekstgebied-extractie ondersteunt, roep #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) aan en genereer één [TemplateField](../../com.groupdocs.parser.templates/templatefield) per niet-lege tekstgebied, genaamd  {prefix}_{n}  (standaardprefix  \"Field\" ). Elk veld krijgt een [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) op de rechthoek van het tekstgebied, waarbij de breedte van de pagina wordt vastgelegd als  pageWidth  zodat latere sjabloonschaling werkt.
3. Als het document geen tekstgebieden ondersteunt, retourneer  null .

### OCR caveat

De C#-implementatie voert OCR uit op de paginavoorvertoning om velden af te leiden wanneer het document alleen uit afbeeldingen bestaat. Java's [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) wordt door de gebruiker geleverd, dus OCR-gedreven generatie is alleen zinvol als er een connector is geconfigureerd EN de connector's  recognizeTextAreas(...)  juiste rechthoeken retourneert. Wanneer  options.getOcrOptions()  is ingesteld en er een connector beschikbaar is, heeft de OCR-pijplijn de voorkeur.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | De generatie-opties. Kan  null  zijn (standaardwaarden toegepast). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Een iterabele van gegenereerde [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s, of  null  als dit niet wordt ondersteund door dit documentformaat.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Extraheert de informatie over alle werkbladen in de spreadsheet.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Een lijst van [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) instanties die informatie bevatten over alle werkbladen in de spreadsheet.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Extraheert de informatie over het werkblad.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | worksheetIndex | int | De nulgebaseerde index van het werkblad. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Extraheert werkbladcellen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | worksheetIndex | int | De nulgebaseerde index van het werkblad. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Een verzameling van [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) instanties die de celgegevens bevatten.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Extraheert werkbladcellen met behulp van aanpassingsopties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | worksheetIndex | int | De nulgebaseerde index van het werkblad. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | De werkblad-extractie-opties. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Een verzameling van [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) instanties die de celgegevens bevatten.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Parseert het document met het door de gebruiker gegenereerde sjabloon.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | De door de gebruiker gegenereerde sjabloon. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Parseert het document met het door de gebruiker gegenereerde sjabloon met de meegeleverde opties.

Als
options.getPageIndex()
is ingesteld, alleen die pagina wordt geparseerd; anders worden alle pagina's geparseerd.

OCR-ondersteuning hangt af van de [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) geconfigureerd in [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | De door de gebruiker gegenereerde sjabloon. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | De parse-by-template opties. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Parseert het document door automatisch de best passende sjabloon uit een collectie te selecteren.

Kopie van de C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
geïntroduceerd in commit 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), en de template die oplevert
het hoogste aantal ingevulde velden (niet‑null paginagebieden met niet‑lege tekst) wint. De C#-implementatie gebruikt
hidden-marker matching tegen een OCR-pas; dat pad is nog niet beschikbaar in Java omdat hidden-field markers en
de OCR‑gedreven TemplatePageOcrParser niet zijn geport, dus deze telling van ingevulde velden wordt gebruikt als een transparante fallback.
Aanroepers die C#-identiek gedrag nodig hebben, moeten een aangepaste selector aansluiten zodra de OCR-engine is gekoppeld.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Een verzameling van kandidaat‑templates. De parser kiest de best passende. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Parse‑opties. Kan null zijn. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Parseert het documentformulier.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Het volgende voorbeeld toont hoe een formulier van het document te parseren:

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


Extraheert gestructureerde tekst uit het document.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - Een instantie van de klasse  org.w3c.dom.Document  met XML‑tekststructuur; null als extractie van tekststructuur niet wordt ondersteund.

### close() {#close--}
```
public void close()
```


Sluit deze bron en geeft alle onderliggende bronnen vrij.


