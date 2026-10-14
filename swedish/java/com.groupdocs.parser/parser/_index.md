---
title: "Parser"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar huvudklassen som kontrollerar extrahering av text‑bilder‑behållare och parsningfunktionalitet."
type: docs
weight: 10
url: /sv/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Representerar huvudklassen som kontrollerar text, bilder, behållarextraktion och parsningfunktionalitet.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL med  loadOptions . |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL med  parserSettings . |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL med  loadOptions  och  parserSettings . |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en databas. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en databas. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions) och [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions) och [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Returnerar den allmänna informationen om en fil. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Returnerar den allmänna informationen om en fil. |
|
|  | [getFeatures()](#getFeatures--) | Hämtar de stödjade funktionerna. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Genererar en förhandsgranskning av en dokumentsida. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Genererar en förhandsgranskning av en dokumentsida med anpassningsalternativ. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Hämta förhandsgranskning av sidor. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Returnerar den allmänna informationen om dokumentet. |
|
|  | [getText()](#getText--) | Extraherar text från dokumentet. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Extraherar en textsida från dokumentet med textalternativ (för att aktivera rått, snabbt textutvinningsläge). |
|
|  | [getText(int pageIndex)](#getText-int-) | Extraherar text från dokumentsidan. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Extraherar text från dokumentsidan med textalternativ (för att aktivera rått, snabbt textutvinningsläge). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Extraherar formaterad text från dokumentet. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Extraherar formaterad text från dokumentsidan. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Söker efter ett nyckelord i dokumentet. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Söker efter ett nyckelord i dokumentet med sökalternativ (reguljärt uttryck, skiftlägeskänslighet, etc.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Extraherar en markering från dokumentet. |
|
|  | [getToc()](#getToc--) | Extraherar en innehållsförteckning från dokumentet. |
|
|  | [getMetadata()](#getMetadata--) | Extraherar metadata från dokumentet. |
|
|  | [getAnnotations()](#getAnnotations--) | Extraherar annotationer från dokumentet. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Extraherar annotationer från dokumentets sida. |
|
|  | [getContainer()](#getContainer--) | Extraherar ett containerobjekt från dokumentet för att arbeta med format som innehåller bilagor, ZIP-arkiv etc. |
|
|  | [getTextAreas()](#getTextAreas--) | Extraherar textområden från dokumentet. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Extraherar textområden från dokumentet med anpassningsalternativ (reguljärt uttryck, skiftlägeskänslighet, etc.). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Extraherar textområden från dokumentets sida. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Extraherar textområden från dokumentets sida med anpassningsalternativ (reguljärt uttryck, skiftlägeskänslighet, etc.). |
|
|  | [getImages()](#getImages--) | Extraherar bilder från dokumentet. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Extraherar bilder från dokumentet med anpassningsalternativ (för att ange det rektangulära området som innehåller bilder). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Extraherar bilder från dokumentets sida. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Extraherar bilder från dokumentets sida med anpassningsalternativ (för att ange det rektangulära området som innehåller bilder). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Extraherar hyperlänkar från dokumentet. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Extraherar hyperlänkar från dokumentets sida. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Extraherar hyperlänkar från dokumentet med anpassningsalternativ (för att ange det rektangulära området som innehåller hyperlänkar). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Extraherar hyperlänkar från dokumentets sida med anpassningsalternativ (för att ange det rektangulära området som innehåller hyperlänkar). |
|
|  | [getBarcodes()](#getBarcodes--) | Extraherar streckkoder från dokumentet. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Extraherar streckkoder från dokumentets sida. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Extraherar streckkoder från dokumentet med anpassningsalternativ (för att ange det rektangulära området som innehåller streckkoder). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Extraherar streckkoder från dokumentets sida med anpassningsalternativ (för att ange det rektangulära området som innehåller streckkoder). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Extraherar tabeller från dokumentet. |
|
|  | [getTables()](#getTables--) | Extraherar tabeller från dokumentet, och upptäcker dem automatiskt. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Extraherar tabeller från dokumentets sida. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Extraherar tabeller från dokumentets sida och upptäcker dem automatiskt. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Genererar en samling av justerings-[TemplateItem](../../com.groupdocs.parser.templates/templateitem)s för dokumentet. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Extraherar informationen om alla arbetsblad i kalkylbladet. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Extraherar informationen om arbetsbladet. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Extraherar celler i arbetsbladet. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Extraherar celler i arbetsbladet med anpassningsalternativ. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Analyserar dokumentet med den användargenererade mallen. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Analyserar dokumentet med den användargenererade mallen och de medföljande alternativen. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Analyserar dokumentet genom att automatiskt välja den bäst matchande mallen från en samling. |
|
|  | [parseForm()](#parseForm--) | Analyserar dokumentformuläret. |
|
|  | [getStructure()](#getStructure--) | Extraherar strukturerad text från dokumentet. |
|
|  | [close()](#close--) | Stänger denna resurs och frigör eventuella underliggande resurser. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | url | java.net.URL | URL:en som begäran skickas till |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL med  loadOptions .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | url | java.net.URL | URL:en som begäran skickas till. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna filen. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL med  parserSettings .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | url | java.net.URL | URL:en som begäran skickas till. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en URL med  loadOptions  och  parserSettings .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | url | java.net.URL | URL:en som begäran skickas till. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna filen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en databas.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Följande exempel visar hur man extraherar data från en Sqlite-databas:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | anslutning | java.sql.Connection | Databasanslutningen. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) för att extrahera data från en databas.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Följande exempel visar hur man extraherar data från en Sqlite-databas:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | anslutning | java.sql.Connection | Databasanslutningen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Följande exempel visar hur man extraherar e-postmeddelanden från Exchange Server:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | E-postanslutningen. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Följande exempel visar hur man extraherar e-postmeddelanden från Exchange Server:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | E-postanslutningen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Följande exempel visar hur man laddar dokumentet från den lokala disken:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Dokumentlösenordet skickas via klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions):

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna filen. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions) och [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Följande exempel visar hur man tar emot informationen via [ILogger](../../com.groupdocs.parser.options/ilogger) gränssnittet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna filen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Följande exempel visar hur man laddar dokumentet från strömmen:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dokument | java.io.InputStream | Källinmatningsströmmen. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

I vissa fall är det nödvändigt att definiera [FileFormat](../../com.groupdocs.parser.options/fileformat). Både för specialfall (databaser, e-postserver)
och för att upptäcka filtyper efter innehållet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dokument | java.io.InputStream | Källinmatningsströmmen. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna filen. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dokument | java.io.InputStream | Källinmatningsströmmen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initierar en ny instans av klassen [Parser](../../com.groupdocs.parser/parser) med [LoadOptions](../../com.groupdocs.parser.options/loadoptions) och [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Följande exempel visar hur man tar emot informationen via [ILogger](../../com.groupdocs.parser.options/ilogger) gränssnittet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dokument | java.io.InputStream | Källinmatningsströmmen. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna filen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Returnerar den allmänna informationen om en fil.

Följande kod visar hur man kontrollerar om en fil är lösenordsskyddad:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Returnerar den allmänna informationen om en fil.

Följande kod visar hur man kontrollerar om en fil är lösenordsskyddad:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dokument | java.io.InputStream | Källinmatningsströmmen. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Hämtar de stödjade funktionerna.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Om funktionen inte stöds, returnerar metoden
null
istället för värdet. Vissa operationer kan förbruka
betydande tid. Så det är inte optimalt att anropa metoden bara för att kontrollera stöd för funktionen.
För detta ändamål används egenskapen Features:

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


Genererar en förhandsgranskning av en dokumentsida.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.io.OutputStream - En instans av java.io.OutputStream som innehåller en bild av dokumentets sida; null om förhandsgranskning av sidan inte stöds.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Genererar en förhandsgranskning av en dokumentsida med anpassningsalternativ.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Alternativen för att anpassa genereringen av förhandsgranskning. |
|

**Returns:**
java.io.OutputStream - En instans av java.io.OutputStream som innehåller en bild av dokumentets sida; null om förhandsgranskning av sidan inte stöds.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Hämta förhandsgranskning av sidor.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Alternativen för att ställa in krav och strömbegäranden för generering av förhandsgranskning. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Returnerar den allmänna informationen om dokumentet.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Följande exempel visar hur man hämtar dokumentinformation:

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


Extraherar text från dokumentet.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Följande exempel visar hur man extraherar text från ett dokument:

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


Extraherar en textsida från dokumentet med textalternativ (för att aktivera rått, snabbt textutvinningsläge).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Följande exempel visar hur man extraherar råtext från ett dokument:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Alternativen för textutdragning. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Extraherar text från dokumentsidan.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Följande exempel visar hur man extraherar text från dokumentets sida:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Extraherar text från dokumentsidan med textalternativ (för att aktivera rått, snabbt textutvinningsläge).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Följande exempel visar hur man extraherar råtext från dokumentets sida:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Alternativen för textutdragning. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Extraherar formaterad text från dokumentet.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Följande exempel visar hur man extraherar dokumenttext som HTML-text:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Alternativen för formaterad textutdragning. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Extraherar formaterad text från dokumentsidan.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Följande exempel visar hur man extraherar en dokumentsidans text som Markdown-text:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Alternativen för formaterad textutdragning. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Söker efter ett nyckelord i dokumentet.

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

Följande exempel visar hur man hittar ett nyckelord i ett dokument:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nyckelord | java.lang.String | Nyckelordet att söka. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - En samling av [SearchResult](../../com.groupdocs.parser.data/searchresult) objekt;  null  om sökning inte stöds.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Söker efter ett nyckelord i dokumentet med sökalternativ (reguljärt uttryck, skiftlägeskänslighet, etc.).

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

Följande exempel visar hur man söker med ett reguljärt uttryck i ett dokument:

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

Följande exempel visar hur man söker en text på sidor:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nyckelord | java.lang.String | Nyckelordet att söka. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Sökalternativen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - En samling av [SearchResult](../../com.groupdocs.parser.data/searchresult) objekt;  null  om sökning inte stöds.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Extraherar en markering från dokumentet.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Följande exempel visar hur man extraherar en markering som innehåller 3 ord:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | int | Startpositionen för markeringen. |
|
|  | isDirect | boolean | Värdet som indikerar om markeringsextraktion är direkt.  true  om markeringen extraheras till höger om positionen; annars,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för markeringsextraktion. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Extraherar en innehållsförteckning från dokumentet.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Följande exempel visar hur man extraherar innehållsförteckning från en EPUB-fil:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - En samling av innehållsförteckningsobjekt;  null  om extraktion av innehållsförteckning inte stöds.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Extraherar metadata från dokumentet.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Följande exempel visar hur man extraherar metadata från ett dokument:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - En samling av metadataobjekt;  null  om metadataextraktion inte stöds.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Extraherar annotationer från dokumentet.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - En samling av annoteringsobjekt;  null  om annoteringsextraktion inte stöds.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Extraherar annotationer från dokumentets sida.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - En samling av annoteringsobjekt;  null  om annoteringsextraktion inte stöds.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Extraherar ett containerobjekt från dokumentet för att arbeta med format som innehåller bilagor, ZIP-arkiv etc.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Följande exempel visar hur man extraherar text från zip‑entiteter:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - En samling av container‑objekt;  null  om containerextraktion inte stöds.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Extraherar textområden från dokumentet.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Följande exempel visar hur man extraherar alla textområden från hela dokumentet:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - En samling av [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objekt;  null  om extraktion av textområden inte stöds.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Extraherar textområden från dokumentet med anpassningsalternativ (reguljärt uttryck, skiftlägeskänslighet, etc.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Följande exempel visar hur man extraherar endast textområden med siffror från det övre vänstra hörnet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Alternativen för extraktion av textområden. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - En samling av [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objekt;  null  om extraktion av textområden inte stöds.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Extraherar textområden från dokumentets sida.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

För att extrahera textområden från en dokumentsida används följande metod:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - En samling av [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objekt;  null  om extraktion av textområden inte stöds.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Extraherar textområden från dokumentets sida med anpassningsalternativ (reguljärt uttryck, skiftlägeskänslighet, etc.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Alternativen för extraktion av textområden. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - En samling av [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objekt;  null  om extraktion av textområden inte stöds.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Extraherar bilder från dokumentet.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Följande exempel visar hur man extraherar alla bilder från hela dokumentet:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - En samling av [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objekt;  null  om bildextraktion inte stöds.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Extraherar bilder från dokumentet med anpassningsalternativ (för att ange det rektangulära området som innehåller bilder).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Följande exempel visar hur man extraherar endast bilder från det övre vänstra hörnet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Alternativen för bildextraktion. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - En samling av [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objekt;  null  om bildextraktion inte stöds.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Extraherar bilder från dokumentets sida.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

För att extrahera bilder från en dokumentsida används följande metod:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - En samling av [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objekt;  null  om bildextraktion inte stöds.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Extraherar bilder från dokumentets sida med anpassningsalternativ (för att ange det rektangulära området som innehåller bilder).

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Alternativen för bildextraktion. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - En samling av [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objekt;  null  om bildextraktion inte stöds.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Extraherar hyperlänkar från dokumentet.

Följande exempel visar hur man extraherar alla hyperlänkar från hela dokumentet:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - En samling av [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objekt;  null  om hyperlänksutdrag inte stöds.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Extraherar hyperlänkar från dokumentets sida.

Följande exempel visar hur man extraherar hyperlänkar från dokumentsidan:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - En samling av [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objekt;  null  om hyperlänksutdrag inte stöds.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Extraherar hyperlänkar från dokumentet med anpassningsalternativ (för att ange det rektangulära området som innehåller hyperlänkar).

Följande exempel visar hur man extraherar hyperlänkar från ett område på dokumentsidan:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Alternativen för hyperlänksutdrag. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - En samling av [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objekt;  null  om hyperlänksutdrag inte stöds.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Extraherar hyperlänkar från dokumentets sida med anpassningsalternativ (för att ange det rektangulära området som innehåller hyperlänkar).

Följande exempel visar hur man extraherar hyperlänkar från ett område på dokumentsidan med anpassningsalternativ:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Alternativen för hyperlänksutdrag. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - En samling av [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objekt;  null  om hyperlänksutdrag inte stöds.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Extraherar streckkoder från dokumentet.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - En samling av [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objekt;  null  om streckkodsextraktion inte stöds.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Extraherar streckkoder från dokumentets sida.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - En samling av [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objekt;  null  om streckkodsextraktion inte stöds.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Extraherar streckkoder från dokumentet med anpassningsalternativ (för att ange det rektangulära området som innehåller streckkoder).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Alternativen för streckkodsextraktion. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - En samling av [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objekt;  null  om streckkodsextraktion inte stöds.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Extraherar streckkoder från dokumentets sida med anpassningsalternativ (för att ange det rektangulära området som innehåller streckkoder).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Alternativen för streckkodsextraktion. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - En samling av [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objekt;  null  om streckkodsextraktion inte stöds.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Extraherar tabeller från dokumentet.

Följande exempel visar hur man extraherar tabeller från hela dokumentet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Alternativen för tabellutdrag. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - En samling av [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objekt;  null  om tabellutdrag inte stöds.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Extraherar tabeller från dokumentet, och upptäcker dem automatiskt.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - En samling av [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objekt;  null  om tabellutdrag inte stöds.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Extraherar tabeller från dokumentets sida.

Följande exempel visar hur man extraherar tabeller från dokumentsidan:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Alternativen för tabellutdrag. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - En samling av [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objekt;  null  om tabellutdrag inte stöds.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Extraherar tabeller från dokumentets sida och upptäcker dem automatiskt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - En samling av [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objekt;  null  om tabellutdrag inte stöds.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Genererar en samling av justerings-[TemplateItem](../../com.groupdocs.parser.templates/templateitem)s för dokumentet.

Java-spegling av C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (commits d4e691b /
ae9e98c). Användbar som en startmall som användaren sedan kan trimma eller byta namn på.

### Algorithm

1. Välj sidan från  options.getPageIndex()  (standard  0 ).
2. Om dokumentet stöder extrahering av textområden, anropa #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) och skapa ett [TemplateField](../../com.groupdocs.parser.templates/templatefield) per icke‑tomt textområde, namngivet  {prefix}_{n}  (standardprefix "Field" ). Varje fält får en [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) i textområdets rektangel, med sidans bredd registrerad som  pageWidth  så att efterföljande mallskalning fungerar.
3. Om dokumentet inte stöder textområden, returnera  null .

### OCR caveat

C#-implementationen kör OCR över sidförhandsvisningen för att härleda fält när dokumentet endast är en bild. Javas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) är användarlevererad, så OCR‑driven generering är bara meningsfull om en anslutning är konfigurerad OCH anslutningens  recognizeTextAreas(...)  returnerar korrekta rektanglar. När  options.getOcrOptions()  är inställd och en anslutning är tillgänglig föredras OCR‑pipeline:n.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Genereringsalternativen. Kan vara  null  (standardvärden tillämpade). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - En iterable av genererade [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s, eller  null  om det inte stöds av detta dokumentformat.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Extraherar informationen om alla arbetsblad i kalkylbladet.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - En lista med [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo)-instanser som innehåller information om alla kalkylblad i kalkylarket.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Extraherar informationen om arbetsbladet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | worksheetIndex | int | Det nollbaserade indexet för kalkylbladet. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Extraherar celler i arbetsbladet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | worksheetIndex | int | Det nollbaserade indexet för kalkylbladet. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - En samling av [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell)-instanser som innehåller celldata.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Extraherar celler i arbetsbladet med anpassningsalternativ.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | worksheetIndex | int | Det nollbaserade indexet för kalkylbladet. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Alternativen för extrahering av kalkylblad. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - En samling av [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell)-instanser som innehåller celldata.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Analyserar dokumentet med den användargenererade mallen.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Den användargenererade mallen. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Analyserar dokumentet med den användargenererade mallen och de medföljande alternativen.

Om
options.getPageIndex()
är angivet, parsas endast den sidan; annars parsas alla sidor.

OCR-stödet beror på den [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) som är konfigurerad i [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Den användargenererade mallen. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Alternativen för parsning efter mall. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Analyserar dokumentet genom att automatiskt välja den bäst matchande mallen från en samling.

Spegel av C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
införd i commit 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), och den mall som ger
det högsta antalet ifyllda fält (icke‑null sidområden med icke‑tom text) vinner. C#‑implementeringen använder
matchning av dolda markörer mot ett OCR-pass; den vägen är ännu inte tillgänglig i Java eftersom dolda fältmarkörer och
den OCR‑drivna TemplatePageOcrParser inte har portats, så detta antal ifyllda fält används som en transparent reserv.
Anropar som behöver exakt C#‑beteende bör ansluta en anpassad selector när OCR‑motorn är ansluten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | En samling av kandidatmallar. Parsaren kommer att välja den som matchar bäst. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Parsningsalternativ. Kan vara null. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Analyserar dokumentformuläret.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Följande exempel visar hur man parsar ett formulär i dokumentet:

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


Extraherar strukturerad text från dokumentet.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - En instans av klassen  org.w3c.dom.Document  med XML‑textstruktur; null om extrahering av textstruktur inte stöds.

### close() {#close--}
```
public void close()
```


Stänger denna resurs och frigör eventuella underliggande resurser.


