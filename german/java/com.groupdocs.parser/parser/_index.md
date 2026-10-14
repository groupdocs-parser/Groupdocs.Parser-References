---
title: "Parser"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Hauptklasse dar, die die Extraktion von Text‑ und Bildcontainern sowie die Parsing‑Funktionalität steuert."
type: docs
weight: 10
url: /de/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Stellt die Hauptklasse dar, die die Text-, Bild-, Container-Extraktion und Parsing-Funktionalität steuert.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL zu extrahieren. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL mit  loadOptions  zu extrahieren. |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL mit  parserSettings  zu extrahieren. |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL mit  loadOptions  und  parserSettings  zu extrahieren. |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten aus einer Datenbank zu extrahieren. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten aus einer Datenbank zu extrahieren. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse. |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse. |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse. |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions) und [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse. |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions) und [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Gibt die allgemeinen Informationen zu einer Datei zurück. |
|
|  | [getFeatures()](#getFeatures--) | Liefert die unterstützten Funktionen. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Erstellt eine Vorschau einer Dokumentenseite. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Erstellt eine Vorschau einer Dokumentenseite unter Verwendung von Anpassungsoptionen. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Seitenvorschau abrufen. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Gibt die allgemeinen Informationen zum Dokument zurück. |
|
|  | [getText()](#getText--) | Extrahiert einen Text aus dem Dokument. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Extrahiert eine Textseite aus dem Dokument mithilfe von Textoptionen (um den rohen schnellen Textextraktionsmodus zu aktivieren). |
|
|  | [getText(int pageIndex)](#getText-int-) | Extrahiert einen Text aus der Dokumentseite. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Extrahiert einen Text aus der Dokumentseite mithilfe von Textoptionen (um den rohen schnellen Textextraktionsmodus zu aktivieren). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Extrahiert einen formatierten Text aus dem Dokument. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Extrahiert einen formatierten Text aus der Dokumentseite. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Sucht ein Schlüsselwort im Dokument. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Sucht ein Schlüsselwort im Dokument mithilfe von Suchoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Extrahiert eine Hervorhebung aus dem Dokument. |
|
|  | [getToc()](#getToc--) | Extrahiert ein Inhaltsverzeichnis aus dem Dokument. |
|
|  | [getMetadata()](#getMetadata--) | Extrahiert Metadaten aus dem Dokument. |
|
|  | [getAnnotations()](#getAnnotations--) | Extrahiert Anmerkungen aus dem Dokument. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Extrahiert Anmerkungen aus der Dokumentseite. |
|
|  | [getContainer()](#getContainer--) | Extrahiert ein Containerobjekt aus dem Dokument, um mit Formaten zu arbeiten, die Anhänge, ZIP-Archive usw. enthalten. |
|
|  | [getTextAreas()](#getTextAreas--) | Extrahiert Textbereiche aus dem Dokument. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Extrahiert Textbereiche aus dem Dokument mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Extrahiert Textbereiche aus der Dokumentseite. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Extrahiert Textbereiche aus der Dokumentseite mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.). |
|
|  | [getImages()](#getImages--) | Extrahiert Bilder aus dem Dokument. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Extrahiert Bilder aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Extrahiert Bilder aus der Dokumentseite. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Extrahiert Bilder aus der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Extrahiert Hyperlinks aus dem Dokument. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Extrahiert Hyperlinks aus der Dokumentseite. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Extrahiert Hyperlinks aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Extrahiert Hyperlinks von der Dokumentseite unter Verwendung von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält). |
|
|  | [getBarcodes()](#getBarcodes--) | Extrahiert Barcodes aus dem Dokument. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Extrahiert Barcodes von der Dokumentseite. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Extrahiert Barcodes aus dem Dokument unter Verwendung von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Extrahiert Barcodes von der Dokumentseite unter Verwendung von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Extrahiert Tabellen aus dem Dokument. |
|
|  | [getTables()](#getTables--) | Extrahiert Tabellen aus dem Dokument und erkennt sie automatisch. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Extrahiert Tabellen von der Dokumentseite. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Extrahiert Tabellen von der Dokumentseite und erkennt sie automatisch. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Erzeugt eine Sammlung von Anpassungs-[TemplateItem](../../com.groupdocs.parser.templates/templateitem)s für das Dokument. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Extrahiert die Informationen über alle Arbeitsblätter in der Kalkulationstabelle. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Extrahiert die Informationen über das Arbeitsblatt. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Extrahiert Zellen des Arbeitsblatts. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Extrahiert Zellen des Arbeitsblatts unter Verwendung von Anpassungsoptionen. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Parst das Dokument mit der vom Benutzer erstellten Vorlage. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Parst das Dokument mit der vom Benutzer erstellten Vorlage und den bereitgestellten Optionen. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Parst das Dokument, indem automatisch die am besten passende Vorlage aus einer Sammlung ausgewählt wird. |
|
|  | [parseForm()](#parseForm--) | Parst das Dokumentformular. |
|
|  | [getStructure()](#getStructure--) | Extrahiert einen strukturierten Text aus dem Dokument. |
|
|  | [close()](#close--) | Schließt diese Ressource und gibt alle zugrunde liegenden Ressourcen frei. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | url | java.net.URL | Die URL, an die die Anfrage gesendet wird |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL mit  loadOptions  zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | url | java.net.URL | Die URL, an die die Anfrage gesendet wird. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen der Datei. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL mit  parserSettings  zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | url | java.net.URL | Die URL, an die die Anfrage gesendet wird. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten von einer URL mit  loadOptions  und  parserSettings  zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | url | java.net.URL | Die URL, an die die Anfrage gesendet wird. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen der Datei. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten aus einer Datenbank zu extrahieren.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Das folgende Beispiel zeigt, wie Daten aus einer Sqlite-Datenbank extrahiert werden:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Verbindung | java.sql.Connection | Die Datenbankverbindung. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse, um Daten aus einer Datenbank zu extrahieren.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Das folgende Beispiel zeigt, wie Daten aus einer Sqlite-Datenbank extrahiert werden:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Verbindung | java.sql.Connection | Die Datenbankverbindung. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Das folgende Beispiel zeigt, wie man E-Mails vom Exchange Server extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Die E-Mail-Verbindung. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Das folgende Beispiel zeigt, wie man E-Mails vom Exchange Server extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Die E-Mail-Verbindung. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Das folgende Beispiel zeigt, wie man das Dokument von der lokalen Festplatte lädt:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Das Dokumentenpasswort wird über die Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) übergeben:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen der Datei. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions) und [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Das folgende Beispiel zeigt, wie man die Informationen über die Schnittstelle [ILogger](../../com.groupdocs.parser.options/ilogger) erhält:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen der Datei. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Das folgende Beispiel zeigt, wie man das Dokument aus dem Stream lädt:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Der Quell-Eingabestream. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

In einigen Fällen ist es notwendig, [FileFormat](../../com.groupdocs.parser.options/fileformat) zu definieren. Sowohl für Sonderfälle (Datenbanken, E-Mail-Server)
als auch zum Erkennen von Dateitypen anhand des Inhalts:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Der Quell-Eingabestream. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen der Datei. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Der Quell-Eingabestream. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initialisiert eine neue Instanz der [Parser](../../com.groupdocs.parser/parser) Klasse mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions) und [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Das folgende Beispiel zeigt, wie man die Informationen über die Schnittstelle [ILogger](../../com.groupdocs.parser.options/ilogger) erhält:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Der Quell-Eingabestream. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen der Datei. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Gibt die allgemeinen Informationen zu einer Datei zurück.

Der folgende Code zeigt, wie man prüft, ob eine Datei passwortgeschützt ist:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Gibt die allgemeinen Informationen zu einer Datei zurück.

Der folgende Code zeigt, wie man prüft, ob eine Datei passwortgeschützt ist:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Der Quell-Eingabestream. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Liefert die unterstützten Funktionen.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Wenn das Feature nicht unterstützt wird, gibt die Methode zurück
null
statt des Wertes. Einige Vorgänge können verbrauchen
signifikante Zeit. Daher ist es nicht optimal, die Methode nur aufzurufen, um die Unterstützung des Features zu prüfen.
Zu diesem Zweck wird die Eigenschaft Features verwendet:

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


Erstellt eine Vorschau einer Dokumentenseite.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.io.OutputStream - Eine Instanz von java.io.OutputStream, die ein Bild der Dokumentenseite enthält;  null  wenn die Generierung der Seitenvorschau nicht unterstützt wird.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Erstellt eine Vorschau einer Dokumentenseite unter Verwendung von Anpassungsoptionen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Die Optionen, um die Vorschaugenerierung anzupassen. |
|

**Returns:**
java.io.OutputStream - Eine Instanz von java.io.OutputStream, die ein Bild der Dokumentenseite enthält;  null  wenn die Generierung der Seitenvorschau nicht unterstützt wird.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Seitenvorschau abrufen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Die Optionen, um Anforderungen und Stream-Delegaten für die Vorschaugenerierung festzulegen. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Gibt die allgemeinen Informationen zum Dokument zurück.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Das folgende Beispiel zeigt, wie man Dokumentinformationen erhält:

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


Extrahiert einen Text aus dem Dokument.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Das folgende Beispiel zeigt, wie man Text aus einem Dokument extrahiert:

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


Extrahiert eine Textseite aus dem Dokument mithilfe von Textoptionen (um den rohen schnellen Textextraktionsmodus zu aktivieren).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Das folgende Beispiel zeigt, wie man Rohtext aus einem Dokument extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Die Optionen zur Textextraktion. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Extrahiert einen Text aus der Dokumentseite.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Das folgende Beispiel zeigt, wie man einen Text aus der Dokumentseite extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Extrahiert einen Text aus der Dokumentseite mithilfe von Textoptionen (um den rohen schnellen Textextraktionsmodus zu aktivieren).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Das folgende Beispiel zeigt, wie man einen Rohtext aus der Dokumentseite extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Die Optionen zur Textextraktion. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Extrahiert einen formatierten Text aus dem Dokument.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Das folgende Beispiel zeigt, wie man einen Dokumenttext als HTML-Text extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Die Optionen für die Extraktion formatierten Textes. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Extrahiert einen formatierten Text aus der Dokumentseite.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Das folgende Beispiel zeigt, wie man einen Dokumentseitentext als Markdown-Text extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Die Optionen für die Extraktion formatierten Textes. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Sucht ein Schlüsselwort im Dokument.

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

Das folgende Beispiel zeigt, wie man ein Schlüsselwort in einem Dokument findet:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Schlüsselwort | java.lang.String | Das zu suchende Schlüsselwort. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Eine Sammlung von [SearchResult](../../com.groupdocs.parser.data/searchresult)-Objekten; null, wenn die Suche nicht unterstützt wird.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Sucht ein Schlüsselwort im Dokument mithilfe von Suchoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.).

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

Das folgende Beispiel zeigt, wie man in einem Dokument mit einem regulären Ausdruck sucht:

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

Das folgende Beispiel zeigt, wie man einen Text auf Seiten sucht:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Schlüsselwort | java.lang.String | Das zu suchende Schlüsselwort. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Die Suchoptionen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Eine Sammlung von [SearchResult](../../com.groupdocs.parser.data/searchresult)-Objekten; null, wenn die Suche nicht unterstützt wird.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Extrahiert eine Hervorhebung aus dem Dokument.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Das folgende Beispiel zeigt, wie man eine Hervorhebung extrahiert, die 3 Wörter enthält:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Position | int | Die Startposition der Hervorhebung. |
|
|  | isDirect | boolean | Der Wert, der angibt, ob die Hervorhebungsextraktion direkt ist. true, wenn die Hervorhebung rechts von der Position extrahiert wird; andernfalls false. |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die Hervorhebungsextraktion. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Extrahiert ein Inhaltsverzeichnis aus dem Dokument.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Das folgende Beispiel zeigt, wie man das Inhaltsverzeichnis aus einer EPUB-Datei extrahiert:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - Eine Sammlung von Inhaltsverzeichnis‑Einträgen; null, wenn die Extraktion des Inhaltsverzeichnisses nicht unterstützt wird.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Extrahiert Metadaten aus dem Dokument.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Das folgende Beispiel zeigt, wie man Metadaten aus einem Dokument extrahiert:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Eine Sammlung von Metadaten‑Einträgen; null, wenn die Metadatenextraktion nicht unterstützt wird.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Extrahiert Anmerkungen aus dem Dokument.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Eine Sammlung von Anmerkungs‑Einträgen; null, wenn die Anmerkungsextraktion nicht unterstützt wird.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Extrahiert Anmerkungen aus der Dokumentseite.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Eine Sammlung von Anmerkungs‑Einträgen; null, wenn die Anmerkungsextraktion nicht unterstützt wird.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Extrahiert ein Containerobjekt aus dem Dokument, um mit Formaten zu arbeiten, die Anhänge, ZIP-Archive usw. enthalten.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Das folgende Beispiel zeigt, wie man einen Text aus ZIP-Entitäten extrahiert:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Eine Sammlung von Container‑Einträgen; null, wenn die Containerextraktion nicht unterstützt wird.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Extrahiert Textbereiche aus dem Dokument.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Das folgende Beispiel zeigt, wie man alle Textbereiche aus dem gesamten Dokument extrahiert:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Eine Sammlung von [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) Objekten; null, wenn die Extraktion von Textbereichen nicht unterstützt wird.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Extrahiert Textbereiche aus dem Dokument mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Das folgende Beispiel zeigt, wie man nur Textbereiche mit Ziffern aus der oberen linken Ecke extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Die Optionen für die Extraktion von Textbereichen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Eine Sammlung von [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) Objekten; null, wenn die Extraktion von Textbereichen nicht unterstützt wird.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Extrahiert Textbereiche aus der Dokumentseite.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Um Textbereiche aus einer Dokumentseite zu extrahieren, wird die folgende Methode verwendet:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Eine Sammlung von [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) Objekten; null, wenn die Extraktion von Textbereichen nicht unterstützt wird.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Extrahiert Textbereiche aus der Dokumentseite mithilfe von Anpassungsoptionen (regulärer Ausdruck, Groß-/Kleinschreibung beachten usw.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Die Optionen für die Extraktion von Textbereichen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Eine Sammlung von [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) Objekten; null, wenn die Extraktion von Textbereichen nicht unterstützt wird.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Extrahiert Bilder aus dem Dokument.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Das folgende Beispiel zeigt, wie man alle Bilder aus dem gesamten Dokument extrahiert:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Eine Sammlung von [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) Objekten; null, wenn die Extraktion von Bildern nicht unterstützt wird.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Extrahiert Bilder aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Das folgende Beispiel zeigt, wie man nur Bilder aus der oberen linken Ecke extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Die Optionen für die Extraktion von Bildern. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Eine Sammlung von [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) Objekten; null, wenn die Extraktion von Bildern nicht unterstützt wird.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Extrahiert Bilder aus der Dokumentseite.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Um Bilder aus einer Dokumentseite zu extrahieren, wird die folgende Methode verwendet:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Eine Sammlung von [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) Objekten; null, wenn die Extraktion von Bildern nicht unterstützt wird.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Extrahiert Bilder aus der Dokumentseite mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Bilder enthält).

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Die Optionen für die Extraktion von Bildern. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Eine Sammlung von [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) Objekten; null, wenn die Extraktion von Bildern nicht unterstützt wird.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Extrahiert Hyperlinks aus dem Dokument.

Das folgende Beispiel zeigt, wie man alle Hyperlinks aus dem gesamten Dokument extrahiert:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Eine Sammlung von [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) Objekten; null, wenn die Extraktion von Hyperlinks nicht unterstützt wird.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Extrahiert Hyperlinks aus der Dokumentseite.

Das folgende Beispiel zeigt, wie man Hyperlinks aus der Dokumentseite extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Eine Sammlung von [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) Objekten; null, wenn die Extraktion von Hyperlinks nicht unterstützt wird.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Extrahiert Hyperlinks aus dem Dokument mithilfe von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält).

Das folgende Beispiel zeigt, wie man Hyperlinks aus dem Dokumentseitenbereich extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Die Optionen für die Extraktion von Hyperlinks. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Eine Sammlung von [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) Objekten; null, wenn die Extraktion von Hyperlinks nicht unterstützt wird.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Extrahiert Hyperlinks von der Dokumentseite unter Verwendung von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Hyperlinks enthält).

Das folgende Beispiel zeigt, wie man Hyperlinks aus dem Dokumentseitenbereich unter Verwendung von Anpassungsoptionen extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Die Optionen für die Extraktion von Hyperlinks. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Eine Sammlung von [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) Objekten; null, wenn die Extraktion von Hyperlinks nicht unterstützt wird.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Extrahiert Barcodes aus dem Dokument.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Eine Sammlung von [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) Objekten; null, wenn die Extraktion von Barcodes nicht unterstützt wird.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Extrahiert Barcodes von der Dokumentseite.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Eine Sammlung von [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) Objekten; null, wenn die Extraktion von Barcodes nicht unterstützt wird.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Extrahiert Barcodes aus dem Dokument unter Verwendung von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Die Optionen für die Extraktion von Barcodes. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Eine Sammlung von [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) Objekten; null, wenn die Extraktion von Barcodes nicht unterstützt wird.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Extrahiert Barcodes von der Dokumentseite unter Verwendung von Anpassungsoptionen (um den rechteckigen Bereich festzulegen, der Barcodes enthält).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Die Optionen für die Extraktion von Barcodes. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Eine Sammlung von [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) Objekten; null, wenn die Extraktion von Barcodes nicht unterstützt wird.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Extrahiert Tabellen aus dem Dokument.

Das folgende Beispiel zeigt, wie man Tabellen aus dem gesamten Dokument extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Die Optionen für die Extraktion von Tabellen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Eine Sammlung von [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) Objekten; null, wenn die Extraktion von Tabellen nicht unterstützt wird.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Extrahiert Tabellen aus dem Dokument und erkennt sie automatisch.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Eine Sammlung von [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) Objekten; null, wenn die Extraktion von Tabellen nicht unterstützt wird.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Extrahiert Tabellen von der Dokumentseite.

Das folgende Beispiel zeigt, wie man Tabellen aus der Dokumentseite extrahiert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Die Optionen für die Extraktion von Tabellen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Eine Sammlung von [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) Objekten; null, wenn die Extraktion von Tabellen nicht unterstützt wird.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Extrahiert Tabellen von der Dokumentseite und erkennt sie automatisch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Eine Sammlung von [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) Objekten; null, wenn die Extraktion von Tabellen nicht unterstützt wird.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Erzeugt eine Sammlung von Anpassungs-[TemplateItem](../../com.groupdocs.parser.templates/templateitem)s für das Dokument.

Java-Spiegel von C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (Commits d4e691b /
ae9e98c). Nützlich als Ausgangsvorlage, die der Benutzer dann kürzen oder umbenennen kann.

### Algorithm

1. Wählen Sie die Seite aus  options.getPageIndex()  (Standard  0 ).
2. Wenn das Dokument die Extraktion von Textbereichen unterstützt, rufen Sie #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) auf und erzeugen Sie ein [TemplateField](../../com.groupdocs.parser.templates/templatefield) pro nicht-leeren Textbereich, benannt {prefix}_{n} (Standardpräfix "Field"). Jeder Bereich erhält ein [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) am Rechteck des Textbereichs, wobei die Seitenbreite als  pageWidth  aufgezeichnet wird, damit die nachfolgende Vorlagenskala funktioniert.
3. Wenn das Dokument keine Textbereiche unterstützt, geben Sie  null  zurück.

### OCR caveat

Die C#-Implementierung führt OCR über die Seitenvorschau aus, um Felder abzuleiten, wenn das Dokument nur aus Bildern besteht. Das [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) von Java wird vom Benutzer bereitgestellt, sodass eine OCR‑gesteuerte Erzeugung nur sinnvoll ist, wenn ein Connector konfiguriert ist UND die Methode des Connectors  recognizeTextAreas(...)  korrekte Rechtecke zurückgibt. Wenn  options.getOcrOptions()  gesetzt ist und ein Connector verfügbar ist, wird die OCR‑Pipeline bevorzugt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Die Generierungsoptionen. Können  null  sein (Standardwerte angewendet). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Ein iterierbares Objekt von erzeugten [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s, oder  null  falls dieses Dokumentformat dies nicht unterstützt.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Extrahiert die Informationen über alle Arbeitsblätter in der Kalkulationstabelle.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Eine Liste von [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo)-Instanzen, die Informationen über alle Arbeitsblätter in der Tabelle enthält.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Extrahiert die Informationen über das Arbeitsblatt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | worksheetIndex | int | Der nullbasierte Index des Arbeitsblatts. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Extrahiert Zellen des Arbeitsblatts.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | worksheetIndex | int | Der nullbasierte Index des Arbeitsblatts. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Eine Sammlung von [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell)-Instanzen, die die Zellen­daten enthält.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Extrahiert Zellen des Arbeitsblatts unter Verwendung von Anpassungsoptionen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | worksheetIndex | int | Der nullbasierte Index des Arbeitsblatts. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Die Optionen zur Arbeitsblattauswertung. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Eine Sammlung von [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell)-Instanzen, die die Zellen­daten enthält.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Parst das Dokument mit der vom Benutzer erstellten Vorlage.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Die vom Benutzer erstellte Vorlage. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Parst das Dokument mit der vom Benutzer erstellten Vorlage und den bereitgestellten Optionen.

Wenn
options.getPageIndex()
ist gesetzt, wird nur diese Seite analysiert; andernfalls werden alle Seiten analysiert.

Die OCR‑Unterstützung hängt vom in [ParserSettings](../../com.groupdocs.parser.options/parsersettings) konfigurierten [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Die vom Benutzer erstellte Vorlage. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Die Optionen zum Parsen nach Vorlage. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Parst das Dokument, indem automatisch die am besten passende Vorlage aus einer Sammlung ausgewählt wird.

Spiegelung von C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
eingeführt im Commit 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), und die Vorlage, die liefert
die höchste Anzahl gefüllter Felder (nicht‑null Seitenbereiche mit nicht‑leeren Texten) gewinnt. Die C#-Implementierung verwendet
Hidden‑Marker‑Abgleich gegen einen OCR‑Durchlauf; dieser Pfad ist in Java noch nicht verfügbar, weil Hidden‑Field‑Marker und
der OCR‑gesteuerte TemplatePageOcrParser nicht portiert sind, daher wird diese Zählung gefüllter Felder als transparenter Rückfall verwendet.
Aufrufer, die ein C#-identisches Verhalten benötigen, sollten einen benutzerdefinierten Selektor einbinden, sobald die OCR-Engine verkabelt ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Eine Sammlung von Kandidatenvorlagen. Der Parser wählt die am besten passende aus. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Kann  null  sein. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Parst das Dokumentformular.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Das folgende Beispiel zeigt, wie man eine Form des Dokuments parst:

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


Extrahiert einen strukturierten Text aus dem Dokument.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - Eine Instanz der  org.w3c.dom.Document  Klasse mit XML-Textstruktur;  null  falls die Extraktion der Textstruktur nicht unterstützt wird.

### close() {#close--}
```
public void close()
```


Schließt diese Ressource und gibt alle zugrunde liegenden Ressourcen frei.


