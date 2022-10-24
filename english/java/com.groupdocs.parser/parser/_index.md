---
title: Parser
second_title: GroupDocs.Parser for Java API Reference
description: Represents the main class that controls text images container extraction and parsing functionality.
type: docs
weight: 10
url: /java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Represents the main class that controls text, images, container extraction and parsing functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [Parser(Connection connection)](#Parser-java.sql.Connection-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class to extract data from a database. |
| [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class to extract data from a database. |
| [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class. |
| [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class. |
| [Parser(String filePath)](#Parser-java.lang.String-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class. |
| [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
| [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
| [Parser(InputStream document)](#Parser-java.io.InputStream-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class. |
| [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
| [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
## Methods

| Method | Description |
| --- | --- |
| [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Returns the general information about a file. |
| [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Returns the general information about a file. |
| [getFeatures()](#getFeatures--) | Gets the supported features. |
| [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Get pages preview. |
| [getDocumentInfo()](#getDocumentInfo--) | Returns the general information about the document. |
| [getText()](#getText--) | Extracts a text from the document. |
| [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Extracts a text page from the document using text options (to enable raw fast text extraction mode). |
| [getText(int pageIndex)](#getText-int-) | Extracts a text from the document page. |
| [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Extracts a text from the document page using text options (to enable raw fast text extraction mode). |
| [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Extracts a formatted text from the document. |
| [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Extracts a formatted text from the document page. |
| [search(String keyword)](#search-java.lang.String-) | Searches a keyword in the document. |
| [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Searches a keyword in the document using search options (regular expression, match case, etc.). |
| [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Extracts a highlight from the document. |
| [getToc()](#getToc--) | Extracts a table of contents from the document. |
| [getMetadata()](#getMetadata--) | Extracts metadata from the document. |
| [getContainer()](#getContainer--) | Extracts a container object from the document to work with formats that contain attachments, ZIP archives etc. |
| [getTextAreas()](#getTextAreas--) | Extracts text areas from the document. |
| [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Extracts text areas from the document using customization options (regular expression, match case, etc.). |
| [getTextAreas(int pageIndex)](#getTextAreas-int-) | Extracts text areas from the document page. |
| [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Extracts text areas from the document page using customization options (regular expression, match case, etc.). |
| [getImages()](#getImages--) | Extracts images from the document. |
| [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Extracts images from the document using customization options (to set the rectangular area that contains images). |
| [getImages(int pageIndex)](#getImages-int-) | Extracts images from the document page. |
| [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Extracts images from the document page using customization options (to set the rectangular area that contains images). |
| [getHyperlinks()](#getHyperlinks--) | Extracts hyperlinks from the document. |
| [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Extracts hyperlinks from the document page. |
| [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Extracts hyperlinks from the document using customization options (to set the rectangular area that contains hyperlinks). |
| [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Extracts hyperlinks from the document page using customization options (to set the rectangular area that contains hyperlinks). |
| [getBarcodes()](#getBarcodes--) | Extracts barcodes from the document. |
| [getBarcodes(int pageIndex)](#getBarcodes-int-) | Extracts barcodes from the document page. |
| [getBarcodes(PageAreaOptions options)](#getBarcodes-com.groupdocs.parser.options.PageAreaOptions-) | Extracts barcodes from the document using customization options (to set the rectangular area that contains barcodes). |
| [getBarcodes(int pageIndex, PageAreaOptions options)](#getBarcodes-int-com.groupdocs.parser.options.PageAreaOptions-) | Extracts barcodes from the document page using customization options (to set the rectangular area that contains barcodes). |
| [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Extracts tables from the document. |
| [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Extracts tables from the document page. |
| [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Parses the document by the user-generated template. |
| [parseForm()](#parseForm--) | Parses the document form. |
| [getStructure()](#getStructure--) | Extracts a structured text from the document. |
| [close()](#close--) | Closes this resource, relinquishing any underlying resources. |
### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class to extract data from a database.

**Learn more:**

 *  [Extract data from databases][]

The following example shows how to extract data from Sqlite database:

```
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
 
```


[Extract data from databases]: https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connection | java.sql.Connection | The database connection. |

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class to extract data from a database.

**Learn more:**

 *  [Extract data from databases][]
 *  [Logging][]

The following example shows how to extract data from Sqlite database:

```
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
 
```


[Extract data from databases]: https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases
[Logging]: https://docs.groupdocs.com/display/parserjava/Logging

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connection | java.sql.Connection | The database connection. |
| parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | The parser settings which are used to customize data extraction. |

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class.

**Learn more:**

 *  [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols][Extract emails from remote server via POP_ IMAP or Exchange Web Services protocols]

The following example shows how to extract emails from Exchange Server:

```
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
 
```


[Extract emails from remote server via POP_ IMAP or Exchange Web Services protocols]: https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | The email connection. |

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class.

**Learn more:**

 *  [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols][Extract emails from remote server via POP_ IMAP or Exchange Web Services protocols]
 *  [Logging][]

The following example shows how to extract emails from Exchange Server:

```
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
 
```


[Extract emails from remote server via POP_ IMAP or Exchange Web Services protocols]: https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols
[Logging]: https://docs.groupdocs.com/display/parserjava/Logging

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | The email connection. |
| parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | The parser settings which are used to customize data extraction. |

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class.

**Learn more:**

 *  [Load document from local disk][]

The following example shows how to load the document from the local disk:

```
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
 
```


[Load document from local disk]: https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The path to the file. |

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

 *  [Load document from local disk][]
 *  [Loading specific file formats][]
 *  [Password-protected documents][]

The document password is passed by [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class:

```
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
 
```


[Load document from local disk]: https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk
[Loading specific file formats]: https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats
[Password-protected documents]: https://docs.groupdocs.com/display/parserjava/Password-protected+documents

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The path to the file. |
| loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | The options to open the file. |

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). and [ParserSettings](../../com.groupdocs.parser.options/parsersettings)

**Learn more:**

 *  [Load document from local disk][]
 *  [Loading specific file formats][]
 *  [Password-protected documents][]
 *  [Logging][]

The following example shows how to receive the information via [ILogger](../../com.groupdocs.parser.options/ilogger) interface:

```
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
 
```


[Load document from local disk]: https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk
[Loading specific file formats]: https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats
[Password-protected documents]: https://docs.groupdocs.com/display/parserjava/Password-protected+documents
[Logging]: https://docs.groupdocs.com/display/parserjava/Logging

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The path to the file. |
| loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | The options to open the file. |
| parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | The parser settings which are used to customize data extraction. |

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class.

**Learn more:**

 *  [Load document from stream][]

The following example shows how to load the document from the stream:

```
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
 
```


[Load document from stream]: https://docs.groupdocs.com/display/parserjava/Load+document+from+stream

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | The source input stream. |

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

 *  [Load document from stream][]
 *  [Loading specific file formats][]
 *  [Password-protected documents][]

In some cases it's necessary to define [FileFormat](../../com.groupdocs.parser.options/fileformat). Both for special cases (databases, email server) and for detecting file types by the content:

```
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
 
```


[Load document from stream]: https://docs.groupdocs.com/display/parserjava/Load+document+from+stream
[Loading specific file formats]: https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats
[Password-protected documents]: https://docs.groupdocs.com/display/parserjava/Password-protected+documents

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | The source input stream. |
| loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | The options to open the file. |

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Initializes a new instance of the [Parser](../../com.groupdocs.parser/parser) class with [LoadOptions](../../com.groupdocs.parser.options/loadoptions). and [ParserSettings](../../com.groupdocs.parser.options/parsersettings)

**Learn more:**

 *  [Load document from stream][]
 *  [Loading specific file formats][]
 *  [Password-protected documents][]
 *  [Logging][]

The following example shows how to receive the information via [ILogger](../../com.groupdocs.parser.options/ilogger) interface:

```
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
 
```


[Load document from stream]: https://docs.groupdocs.com/display/parserjava/Load+document+from+stream
[Loading specific file formats]: https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats
[Password-protected documents]: https://docs.groupdocs.com/display/parserjava/Password-protected+documents
[Logging]: https://docs.groupdocs.com/display/parserjava/Logging

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | The source input stream. |
| loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | The options to open the file. |
| parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | The parser settings which are used to customize data extraction. |

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Returns the general information about a file.

The following code shows how to check whether a file is password-protected:

```
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The path to the file. |

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.
### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Returns the general information about a file.

The following code shows how to check whether a file is password-protected:

```
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | The source input stream. |

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.
### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Gets the supported features.

**Learn more:**

 *  [Get supported features][]

If the feature isn't supported, the method returns  null  instead of the value. Some operations may consume significant time. So it's not optimal to call the method to just check the support for the feature. For this purpose Features property is used:

```
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
 
```


[Get supported features]: https://docs.groupdocs.com/display/parserjava/Get+supported+features

**Returns:**
[Features](../../com.groupdocs.parser.options/features) - An instance of [Features](../../com.groupdocs.parser.options/features) class that represents the supported features.
### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Get pages preview.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | The options to sets requirements and stream delegates for preview generation. |

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Returns the general information about the document.

**Learn more:**

 *  [Get document info][]
 *  [Detect encoding][]

The following example shows how to get document info:

```
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Get the document info
     IDocumentInfo info = parser.getDocumentInfo();
     // Print document information
     System.out.println(String.format("FileType: %s", info.getFileType()));
     System.out.println(String.format("PageCount: %d", info.getPageCount()));
     System.out.println(String.format("Size: %d", info.getSize()));
 }
 
```


[Get document info]: https://docs.groupdocs.com/display/parserjava/Get+document+info
[Detect encoding]: https://docs.groupdocs.com/display/parserjava/Detect+encoding

**Returns:**
[IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) - An instance of class that implements [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) interface.
### getText() {#getText--}
```
public TextReader getText()
```


Extracts a text from the document.

**Learn more:**

 *  [Extract text from documents][]
 *  [Extract text in Accurate Mode][]

The following example shows how to extract a text from a document:

```
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a text into the reader
     try (TextReader reader = parser.getText()) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
```


[Extract text from documents]: https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents
[Extract text in Accurate Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.
### getText(TextOptions options) {#getText-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(TextOptions options)
```


Extracts a text page from the document using text options (to enable raw fast text extraction mode).

**Learn more:**

 *  [Extract text in Raw Mode][]
 *  [Extract text in Accurate Mode][]

The following example shows how to extract a raw text from a document:

```
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SamplePdf)) {
     // Extract a raw text into the reader
     try (TextReader reader = parser.getText(new TextOptions(true))) {
         // Print a text from the document
         // If text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Text extraction isn't supported" : reader.readToEnd());
     }
 }
 
```


[Extract text in Raw Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode
[Extract text in Accurate Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | The text extraction options. |

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.
### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Extracts a text from the document page.

**Learn more:**

 *  [Extract text in Accurate Mode][]

The following example shows how to extract a text from the document page:

```
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
 
```


[Extract text in Accurate Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.
### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Extracts a text from the document page using text options (to enable raw fast text extraction mode).

**Learn more:**

 *  [Extract text in Raw Mode][]
 *  [Extract text in Accurate Mode][]

The following example shows how to extract a raw text from the document page:

```
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
 
```


[Extract text in Raw Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode
[Extract text in Accurate Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | The text extraction options. |

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.
### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Extracts a formatted text from the document.

**Learn more:**

 *  [Extract formatted text from document][]
 *  Extract a document text as [HTML][]
 *  Extract a document text as [Markdown][]
 *  Extract a document text as [Plain text][]

The following example shows how to extract a document text as HTML text:

```
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocx)) {
     // Extract a formatted text into the reader
     try (TextReader reader = parser.getFormattedText(new FormattedTextOptions(FormattedTextMode.Html))) {
         // Print a formatted text from the document
         // If formatted text extraction isn't supported, a reader is null
         System.out.println(reader == null ? "Formatted text extraction isn't suppported" : reader.readToEnd());
     }
 }
 
```


[Extract formatted text from document]: https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document
[HTML]: https://docs.groupdocs.com/display/parserjava/HTML
[Markdown]: https://docs.groupdocs.com/display/parserjava/Markdown
[Plain text]: https://docs.groupdocs.com/display/parserjava/Plain+text

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | The formatted text extraction options. |

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.
### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Extracts a formatted text from the document page.

**Learn more:**

 *  [Extract formatted text from document page][]
 *  Extract a document text as [HTML][]
 *  Extract a document text as [Markdown][]
 *  Extract a document text as [Plain text][]

The following example shows how to extract a document page text as Markdown text:

```
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
 
```


[Extract formatted text from document page]: https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page
[HTML]: https://docs.groupdocs.com/display/parserjava/HTML
[Markdown]: https://docs.groupdocs.com/display/parserjava/Markdown
[Plain text]: https://docs.groupdocs.com/display/parserjava/Plain+text

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | The formatted text extraction options. |

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.
### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Searches a keyword in the document.

**Learn more:**

 *  [Search text][]
 *  [Search text in Microsoft Office Word documents][]
 *  [Search text in Microsoft Office Excel spreadsheets][]
 *  [Search text in Microsoft Office PowerPoint presentations][]
 *  [Search text in PDF documents][]
 *  [Search text in Emails][]
 *  [Search text in EPUB eBooks][]
 *  [Search text in HTML documents][]
 *  [Search text in Microsoft OneNote sections][]

The following example shows how to find a keyword in a document:

```
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
 
```


[Search text]: https://docs.groupdocs.com/display/parserjava/Search+text
[Search text in Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents
[Search text in Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets
[Search text in Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations
[Search text in PDF documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents
[Search text in Emails]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails
[Search text in EPUB eBooks]: https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks
[Search text in HTML documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents
[Search text in Microsoft OneNote sections]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| keyword | java.lang.String | The keyword to search. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - A collection of [SearchResult](../../com.groupdocs.parser.data/searchresult) objects;  null  if search isn't supported.
### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Searches a keyword in the document using search options (regular expression, match case, etc.).

**Learn more:**

 *  [Search text][]
 *  [Search text in Microsoft Office Word documents][]
 *  [Search text in Microsoft Office Excel spreadsheets][]
 *  [Search text in Microsoft Office PowerPoint presentations][]
 *  [Search text in PDF documents][]
 *  [Search text in Emails][]
 *  [Search text in EPUB eBooks][]
 *  [Search text in HTML documents][]
 *  [Search text in Microsoft OneNote sections][]

The following example shows how to search with a regular expression in a document:

```
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
 
```

The following example shows how to search a text on pages:

```
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
 
```


[Search text]: https://docs.groupdocs.com/display/parserjava/Search+text
[Search text in Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents
[Search text in Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets
[Search text in Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations
[Search text in PDF documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents
[Search text in Emails]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails
[Search text in EPUB eBooks]: https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks
[Search text in HTML documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents
[Search text in Microsoft OneNote sections]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| keyword | java.lang.String | The keyword to search. |
| options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | The search options. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - A collection of [SearchResult](../../com.groupdocs.parser.data/searchresult) objects;  null  if search isn't supported.
### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Extracts a highlight from the document.

**Learn more:**

 *  [Extract highlights][]

The following example shows how to extract a highlight that contains 3 words:

```
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
 
```


[Extract highlights]: https://docs.groupdocs.com/display/parserjava/Extract+highlights

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | int | The start position of the highlight. |
| isDirect | boolean | The value that indicates whether highlight extraction is direct.  true  if the higlight is extracted by the right of position; otherwise,  false . |
| options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | The highlight extraction options. |

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.
### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Extracts a table of contents from the document.

**Learn more:**

 *  [Extract table of contents][]
 *  [Extract text by table of contents item][]
 *  [Extract table of contents from Microsoft Office Word documents][]
 *  [Extract table of contents from EPUB eBooks][]

The following example shows how to extract table of contents from EPUB file:

```
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
 
```


[Extract table of contents]: https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents
[Extract text by table of contents item]: https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item
[Extract table of contents from Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents
[Extract table of contents from EPUB eBooks]: https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - A collection of table of contents items;  null  if table of contents extraction isn't supported.
### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Extracts metadata from the document.

**Learn more:**

 *  [Extract metadata from documents][]
 *  [Extract metadata from Microsoft Office Word documents][]
 *  [Extract metadata from Microsoft Office Excel spreadsheets][]
 *  [Extract metadata from Microsoft Office PowerPoint presentations][]
 *  [Extract metadata from PDF documents][]
 *  [Extract metadata from Emails][]

The following example shows how to extract metadata from a document:

```
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
 
```


[Extract metadata from documents]: https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents
[Extract metadata from Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents
[Extract metadata from Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets
[Extract metadata from Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations
[Extract metadata from PDF documents]: https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents
[Extract metadata from Emails]: https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - A collection of metadata items;  null  if metadata extraction isn't supported.
### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Extracts a container object from the document to work with formats that contain attachments, ZIP archives etc.

**Learn more:**

 *  [Extract data from attachments and ZIP archives][]
 *  [Iterate through container items][]
 *  [Extract attachments from PDF portfolios][]
 *  [Extract attachments from Emails][]
 *  [Extract emails from Outlook Storage][]
 *  [Extract text from ZIP archive files][]

The following example shows how to extract a text from zip entities:

```
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
 
```


[Extract data from attachments and ZIP archives]: https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives
[Iterate through container items]: https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items
[Extract attachments from PDF portfolios]: https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios
[Extract attachments from Emails]: https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails
[Extract emails from Outlook Storage]: https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage
[Extract text from ZIP archive files]: https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - A collection of container items;  null  if container extraction isn't supported.
### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Extracts text areas from the document.

**Learn more:**

 *  [Extract text areas][]

The following example shows how to extract all text areas from the whole document:

```
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
 
```


[Extract text areas]: https://docs.groupdocs.com/display/parserjava/Extract+text+areas

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - A collection of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objects;  null  if text areas extraction isn't supported.
### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Extracts text areas from the document using customization options (regular expression, match case, etc.).

**Learn more:**

 *  [Extract text areas][]

The following example shows how to extract only text areas with digits from the upper-left courner:

```
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
 
```


[Extract text areas]: https://docs.groupdocs.com/display/parserjava/Extract+text+areas

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | The options for text area extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - A collection of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objects;  null  if text areas extraction isn't supported.
### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Extracts text areas from the document page.

**Learn more:**

 *  [Extract text areas][]

To extract text areas from a document page the following method is used:

```
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
 
```


[Extract text areas]: https://docs.groupdocs.com/display/parserjava/Extract+text+areas

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - A collection of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objects;  null  if text areas extraction isn't supported.
### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Extracts text areas from the document page using customization options (regular expression, match case, etc.).

**Learn more:**

 *  [Extract text areas][]


[Extract text areas]: https://docs.groupdocs.com/display/parserjava/Extract+text+areas

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | The options for text area extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - A collection of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objects;  null  if text areas extraction isn't supported.
### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Extracts images from the document.

**Learn more:**

 *  [Extract images from documents][]
 *  [Extract images to files][]
 *  [Extract images from Microsoft Office Word documents][]
 *  [Extract images from Microsoft Office Excel spreadsheets][]
 *  [Extract images from Microsoft Office PowerPoint presentations][]
 *  [Extract images from Emails][]
 *  [Extract images from PDF documents][]

The following example shows how to extract all images from the whole document:

```
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
 
```


[Extract images from documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents
[Extract images to files]: https://docs.groupdocs.com/display/parserjava/Extract+images+to+files
[Extract images from Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents
[Extract images from Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets
[Extract images from Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations
[Extract images from Emails]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails
[Extract images from PDF documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - A collection of [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objects;  null  if images extraction isn't supported.
### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Extracts images from the document using customization options (to set the rectangular area that contains images).

**Learn more:**

 *  [Extract images from documents][]
 *  [Extract images to files][]
 *  [Extract images from document page area][]
 *  [Extract images from Microsoft Office Word documents][]
 *  [Extract images from Microsoft Office Excel spreadsheets][]
 *  [Extract images from Microsoft Office PowerPoint presentations][]
 *  [Extract images from Emails][]
 *  [Extract images from PDF documents][]

The following example shows how to extract only images from the upper-left courner:

```
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
 
```


[Extract images from documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents
[Extract images to files]: https://docs.groupdocs.com/display/parserjava/Extract+images+to+files
[Extract images from document page area]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area
[Extract images from Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents
[Extract images from Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets
[Extract images from Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations
[Extract images from Emails]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails
[Extract images from PDF documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | The options for images extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - A collection of [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objects;  null  if images extraction isn't supported.
### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Extracts images from the document page.

**Learn more:**

 *  [Extract images from documents][]
 *  [Extract images to files][]
 *  [Extract images from document page][]
 *  [Extract images from Microsoft Office Word documents][]
 *  [Extract images from Microsoft Office Excel spreadsheets][]
 *  [Extract images from Microsoft Office PowerPoint presentations][]
 *  [Extract images from Emails][]
 *  [Extract images from PDF documents][]

To extract images from a document page the following method is used:

```
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
 
```


[Extract images from documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents
[Extract images to files]: https://docs.groupdocs.com/display/parserjava/Extract+images+to+files
[Extract images from document page]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page
[Extract images from Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents
[Extract images from Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets
[Extract images from Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations
[Extract images from Emails]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails
[Extract images from PDF documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - A collection of [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objects;  null  if images extraction isn't supported.
### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Extracts images from the document page using customization options (to set the rectangular area that contains images).

**Learn more:**

 *  [Extract images from documents][]
 *  [Extract images to files][]
 *  [Extract images from document page][]
 *  [Extract images from document page area][]
 *  [Extract images from Microsoft Office Word documents][]
 *  [Extract images from Microsoft Office Excel spreadsheets][]
 *  [Extract images from Microsoft Office PowerPoint presentations][]
 *  [Extract images from Emails][]
 *  [Extract images from PDF documents][]


[Extract images from documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents
[Extract images to files]: https://docs.groupdocs.com/display/parserjava/Extract+images+to+files
[Extract images from document page]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page
[Extract images from document page area]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area
[Extract images from Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents
[Extract images from Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets
[Extract images from Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations
[Extract images from Emails]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails
[Extract images from PDF documents]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | The options for images extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - A collection of [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) objects;  null  if images extraction isn't supported.
### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Extracts hyperlinks from the document.

The following example shows how to extract all hyperlinks from the whole document:

```
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
 
```

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - A collection of [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objects;  null  if hyperlinks extraction isn't supported.
### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Extracts hyperlinks from the document page.

The following example shows how to extract hyperlinks from the document page:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - A collection of [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objects;  null  if hyperlinks extraction isn't supported.
### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Extracts hyperlinks from the document using customization options (to set the rectangular area that contains hyperlinks).

The following example shows how to extract hyperlinks from the document page area:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | The options for hyperlinks extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - A collection of [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objects;  null  if hyperlinks extraction isn't supported.
### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Extracts hyperlinks from the document page using customization options (to set the rectangular area that contains hyperlinks).

The following example shows how to extract hyperlinks from the document page area using customization options:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | The options for hyperlinks extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - A collection of [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) objects;  null  if hyperlinks extraction isn't supported.
### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Extracts barcodes from the document.

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - A collection of [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objects;  null  if barcodes extraction isn't supported.
### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Extracts barcodes from the document page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - A collection of [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objects;  null  if barcodes extraction isn't supported.
### getBarcodes(PageAreaOptions options) {#getBarcodes-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(PageAreaOptions options)
```


Extracts barcodes from the document using customization options (to set the rectangular area that contains barcodes).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | The options for barcodes extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - A collection of [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objects;  null  if barcodes extraction isn't supported.
### getBarcodes(int pageIndex, PageAreaOptions options) {#getBarcodes-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, PageAreaOptions options)
```


Extracts barcodes from the document page using customization options (to set the rectangular area that contains barcodes).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | The options for barcodes extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - A collection of [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) objects;  null  if barcodes extraction isn't supported.
### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Extracts tables from the document.

The following example shows how to extract tables from the whole document:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | The options for tables extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - A collection of [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objects;  null  if tables extraction isn't supported.
### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Extracts tables from the document page.

The following example shows how to extract tables from the document page:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | The options for tables extraction. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - A collection of [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) objects;  null  if tables extraction isn't supported.
### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Parses the document by the user-generated template.

**Learn more:**

 *  [Parse data from documents][]
 *  [Working with templates][]
 *  [Working with data extracted by template][]
 *  [Parse data from PDF documents][]


[Parse data from documents]: https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents
[Working with templates]: https://docs.groupdocs.com/display/parserjava/Working+with+templates
[Working with data extracted by template]: https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template
[Parse data from PDF documents]: https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| template | [Template](../../com.groupdocs.parser.templates/template) | The user-generated template. |

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.
### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Parses the document form.

**Learn more:**

 *  [Extract data from PDF forms][]
 *  [Working with data extracted by template][]
 *  [Parse data from PDF documents][]

The following example shows how to parse a form of the document:

```
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
 
```


[Extract data from PDF forms]: https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms
[Working with data extracted by template]: https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template
[Parse data from PDF documents]: https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.
### getStructure() {#getStructure--}
```
public Document getStructure()
```


Extracts a structured text from the document.

**Learn more:**

 *  [Extract text structure][]


[Extract text structure]: https://docs.groupdocs.com/display/parserjava/Extract+text+structure

**Returns:**
org.w3c.dom.Document - An instance of  org.w3c.dom.Document  class with XML text structure;  null  if text structure extraction isn't supported.
### close() {#close--}
```
public void close()
```


Closes this resource, relinquishing any underlying resources.

