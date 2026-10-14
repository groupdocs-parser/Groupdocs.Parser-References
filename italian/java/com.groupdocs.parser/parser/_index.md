---
title: "Parser"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta la classe principale che controlla l'estrazione del contenitore di immagini di testo e la funzionalità di parsing."
type: docs
weight: 10
url: /it/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Rappresenta la classe principale che controlla la funzionalità di estrazione e analisi di testo, immagini e contenitori.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL con  loadOptions . |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL con  parserSettings . |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL con  loadOptions  e  parserSettings . |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un database. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un database. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) e [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) e [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Restituisce le informazioni generali su un file. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Restituisce le informazioni generali su un file. |
|
|  | [getFeatures()](#getFeatures--) | Ottiene le funzionalità supportate. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Genera un'anteprima della pagina del documento. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Genera un'anteprima della pagina del documento utilizzando le opzioni di personalizzazione. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Ottieni l'anteprima delle pagine. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Restituisce le informazioni generali sul documento. |
|
|  | [getText()](#getText--) | Estrae un testo dal documento. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Estrae una pagina di testo dal documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo). |
|
|  | [getText(int pageIndex)](#getText-int-) | Estrae un testo dalla pagina del documento. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Estrae un testo dalla pagina del documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Estrae un testo formattato dal documento. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Estrae un testo formattato dalla pagina del documento. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Cerca una parola chiave nel documento. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Cerca una parola chiave nel documento utilizzando le opzioni di ricerca (espressione regolare, distinzione maiuscole/minuscole, ecc.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Estrae un evidenziato dal documento. |
|
|  | [getToc()](#getToc--) | Estrae un indice dal documento. |
|
|  | [getMetadata()](#getMetadata--) | Estrae i metadati dal documento. |
|
|  | [getAnnotations()](#getAnnotations--) | Estrae le annotazioni dal documento. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Estrae le annotazioni dalla pagina del documento. |
|
|  | [getContainer()](#getContainer--) | Estrae un oggetto contenitore dal documento per lavorare con formati che contengono allegati, archivi ZIP ecc. |
|
|  | [getTextAreas()](#getTextAreas--) | Estrae le aree di testo dal documento. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Estrae le aree di testo dal documento usando opzioni di personalizzazione (espressione regolare, distinzione tra maiuscole e minuscole, ecc.). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Estrae le aree di testo dalla pagina del documento. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Estrae le aree di testo dalla pagina del documento usando opzioni di personalizzazione (espressione regolare, distinzione tra maiuscole e minuscole, ecc.). |
|
|  | [getImages()](#getImages--) | Estrae le immagini dal documento. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Estrae le immagini dal documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Estrae le immagini dalla pagina del documento. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Estrae le immagini dalla pagina del documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Estrae i collegamenti ipertestuali dal documento. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Estrae i collegamenti ipertestuali dalla pagina del documento. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Estrae i collegamenti ipertestuali dal documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Estrae i collegamenti ipertestuali dalla pagina del documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali). |
|
|  | [getBarcodes()](#getBarcodes--) | Estrae i codici a barre dal documento. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Estrae i codici a barre dalla pagina del documento. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Estrae i codici a barre dal documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Estrae i codici a barre dalla pagina del documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Estrae le tabelle dal documento. |
|
|  | [getTables()](#getTables--) | Estrae le tabelle dal documento, rilevandole automaticamente. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Estrae le tabelle dalla pagina del documento. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Estrae le tabelle dalla pagina del documento, rilevandole automaticamente. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Genera una raccolta di [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s di regolazione per il documento. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Estrae le informazioni su tutti i fogli di lavoro nel foglio di calcolo. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Estrae le informazioni sul foglio di lavoro. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Estrae le celle del foglio di lavoro. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Estrae le celle del foglio di lavoro usando opzioni di personalizzazione. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Analizza il documento con il modello generato dall'utente. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Analizza il documento con il modello generato dall'utente utilizzando le opzioni fornite. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Analizza il documento selezionando automaticamente il modello più adatto da una raccolta. |
|
|  | [parseForm()](#parseForm--) | Analizza il modulo del documento. |
|
|  | [getStructure()](#getStructure--) | Estrae un testo strutturato dal documento. |
|
|  | [close()](#close--) | Chiude questa risorsa, rilasciando eventuali risorse sottostanti. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | url | java.net.URL | L'URL a cui viene inviata la richiesta |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL con  loadOptions .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | url | java.net.URL | L'URL a cui viene inviata la richiesta. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il file. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL con  parserSettings .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | url | java.net.URL | L'URL a cui viene inviata la richiesta. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un URL con  loadOptions  e  parserSettings .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | url | java.net.URL | L'URL a cui viene inviata la richiesta. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un database.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Il seguente esempio mostra come estrarre dati da un database Sqlite:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | connessione | java.sql.Connection | La connessione al database. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) per estrarre dati da un database.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Il seguente esempio mostra come estrarre dati da un database Sqlite:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | connessione | java.sql.Connection | La connessione al database. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Il seguente esempio mostra come estrarre email da Exchange Server:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | La connessione email. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Il seguente esempio mostra come estrarre email da Exchange Server:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | La connessione email. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Il seguente esempio mostra come caricare il documento dal disco locale:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

La password del documento è passata dalla classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions):

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il file. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) e [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Il seguente esempio mostra come ricevere le informazioni tramite l'interfaccia [ILogger](../../com.groupdocs.parser.options/ilogger):

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Il seguente esempio mostra come caricare il documento dallo stream:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Lo stream di input di origine. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

In alcuni casi è necessario definire [FileFormat](../../com.groupdocs.parser.options/fileformat). Sia per casi speciali (database, server di posta elettronica)
e per rilevare i tipi di file in base al contenuto:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Lo stream di input di origine. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il file. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Lo stream di input di origine. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Inizializza una nuova istanza della classe [Parser](../../com.groupdocs.parser/parser) con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) e [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Il seguente esempio mostra come ricevere le informazioni tramite l'interfaccia [ILogger](../../com.groupdocs.parser.options/ilogger):

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Lo stream di input di origine. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il file. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Restituisce le informazioni generali su un file.

Il seguente codice mostra come verificare se un file è protetto da password:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Restituisce le informazioni generali su un file.

Il seguente codice mostra come verificare se un file è protetto da password:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documento | java.io.InputStream | Lo stream di input di origine. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Ottiene le funzionalità supportate.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Se la funzionalità non è supportata, il metodo restituisce
null
invece del valore. Alcune operazioni possono consumare
tempo significativo. Quindi non è ottimale chiamare il metodo solo per verificare il supporto della funzionalità.
Per questo scopo viene utilizzata la proprietà Features:

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


Genera un'anteprima della pagina del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.io.OutputStream - Un'istanza di java.io.OutputStream contenente un'immagine della pagina del documento;  null  se la generazione dell'anteprima della pagina non è supportata.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Genera un'anteprima della pagina del documento utilizzando le opzioni di personalizzazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Le opzioni per personalizzare la generazione dell'anteprima. |
|

**Returns:**
java.io.OutputStream - Un'istanza di java.io.OutputStream contenente un'immagine della pagina del documento;  null  se la generazione dell'anteprima della pagina non è supportata.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Ottieni l'anteprima delle pagine.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Le opzioni per impostare requisiti e delegati di flusso per la generazione dell'anteprima. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Restituisce le informazioni generali sul documento.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Il seguente esempio mostra come ottenere le informazioni del documento:

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


Estrae un testo dal documento.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Il seguente esempio mostra come estrarre del testo da un documento:

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


Estrae una pagina di testo dal documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Il seguente esempio mostra come estrarre un testo grezzo da un documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Le opzioni di estrazione del testo. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Estrae un testo dalla pagina del documento.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Il seguente esempio mostra come estrarre del testo dalla pagina del documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Estrae un testo dalla pagina del documento utilizzando le opzioni di testo (per abilitare la modalità di estrazione rapida di testo grezzo).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Il seguente esempio mostra come estrarre un testo grezzo dalla pagina del documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Le opzioni di estrazione del testo. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Estrae un testo formattato dal documento.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Il seguente esempio mostra come estrarre il testo del documento come testo HTML:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Le opzioni di estrazione del testo formattato. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Estrae un testo formattato dalla pagina del documento.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Il seguente esempio mostra come estrarre il testo della pagina del documento come testo Markdown:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Le opzioni di estrazione del testo formattato. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Cerca una parola chiave nel documento.

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

Il seguente esempio mostra come trovare una parola chiave in un documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola chiave | java.lang.String | La parola chiave da cercare. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Una collezione di oggetti [SearchResult](../../com.groupdocs.parser.data/searchresult);  null  se la ricerca non è supportata.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Cerca una parola chiave nel documento utilizzando le opzioni di ricerca (espressione regolare, distinzione maiuscole/minuscole, ecc.).

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

Il seguente esempio mostra come cercare con un'espressione regolare in un documento:

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

Il seguente esempio mostra come cercare del testo nelle pagine:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola chiave | java.lang.String | La parola chiave da cercare. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Le opzioni di ricerca. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - Una collezione di oggetti [SearchResult](../../com.groupdocs.parser.data/searchresult);  null  se la ricerca non è supportata.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Estrae un evidenziato dal documento.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Il seguente esempio mostra come estrarre un'evidenziazione che contiene 3 parole:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | posizione | int | La posizione iniziale dell'evidenziazione. |
|
|  | isDirect | boolean | Il valore che indica se l'estrazione dell'evidenziazione è diretta.  true  se l'evidenziazione è estratta a destra della posizione; altrimenti,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Le opzioni di estrazione dell'evidenziazione. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Estrae un indice dal documento.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Il seguente esempio mostra come estrarre il sommario da un file EPUB:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - Una collezione di elementi del sommario;  null  se l'estrazione del sommario non è supportata.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Estrae i metadati dal documento.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Il seguente esempio mostra come estrarre i metadati da un documento:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Una collezione di elementi di metadati;  null  se l'estrazione dei metadati non è supportata.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Estrae le annotazioni dal documento.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Una collezione di elementi di annotazione;  null  se l'estrazione delle annotazioni non è supportata.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Estrae le annotazioni dalla pagina del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Una collezione di elementi di annotazione;  null  se l'estrazione delle annotazioni non è supportata.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Estrae un oggetto contenitore dal documento per lavorare con formati che contengono allegati, archivi ZIP ecc.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Il seguente esempio mostra come estrarre un testo da entità zip:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Una collezione di elementi del contenitore;  null  se l'estrazione del contenitore non è supportata.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Estrae le aree di testo dal documento.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Il seguente esempio mostra come estrarre tutte le aree di testo dall'intero documento:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Una collezione di oggetti [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  se l'estrazione delle aree di testo non è supportata.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Estrae le aree di testo dal documento usando opzioni di personalizzazione (espressione regolare, distinzione tra maiuscole e minuscole, ecc.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Il seguente esempio mostra come estrarre solo le aree di testo con cifre dall'angolo in alto a sinistra:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Le opzioni per l'estrazione delle aree di testo. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Una collezione di oggetti [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  se l'estrazione delle aree di testo non è supportata.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Estrae le aree di testo dalla pagina del documento.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Per estrarre le aree di testo da una pagina del documento si utilizza il seguente metodo:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Una collezione di oggetti [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  se l'estrazione delle aree di testo non è supportata.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Estrae le aree di testo dalla pagina del documento usando opzioni di personalizzazione (espressione regolare, distinzione tra maiuscole e minuscole, ecc.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Le opzioni per l'estrazione delle aree di testo. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Una collezione di oggetti [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  se l'estrazione delle aree di testo non è supportata.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Estrae le immagini dal documento.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Il seguente esempio mostra come estrarre tutte le immagini dall'intero documento:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Una collezione di oggetti [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  se l'estrazione delle immagini non è supportata.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Estrae le immagini dal documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Il seguente esempio mostra come estrarre solo le immagini dall'angolo in alto a sinistra:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Le opzioni per l'estrazione delle immagini. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Una collezione di oggetti [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  se l'estrazione delle immagini non è supportata.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Estrae le immagini dalla pagina del documento.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Per estrarre le immagini da una pagina del documento si utilizza il seguente metodo:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Una collezione di oggetti [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  se l'estrazione delle immagini non è supportata.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Estrae le immagini dalla pagina del documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene le immagini).

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Le opzioni per l'estrazione delle immagini. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Una collezione di oggetti [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  se l'estrazione delle immagini non è supportata.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Estrae i collegamenti ipertestuali dal documento.

Il seguente esempio mostra come estrarre tutti i collegamenti ipertestuali dall'intero documento:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Una collezione di oggetti [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  se l'estrazione dei collegamenti ipertestuali non è supportata.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Estrae i collegamenti ipertestuali dalla pagina del documento.

Il seguente esempio mostra come estrarre i collegamenti ipertestuali dalla pagina del documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Una collezione di oggetti [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  se l'estrazione dei collegamenti ipertestuali non è supportata.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Estrae i collegamenti ipertestuali dal documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali).

Il seguente esempio mostra come estrarre i collegamenti ipertestuali dall'area della pagina del documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Le opzioni per l'estrazione dei collegamenti ipertestuali. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Una collezione di oggetti [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  se l'estrazione dei collegamenti ipertestuali non è supportata.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Estrae i collegamenti ipertestuali dalla pagina del documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i collegamenti ipertestuali).

Il seguente esempio mostra come estrarre i collegamenti ipertestuali dall'area della pagina del documento utilizzando le opzioni di personalizzazione:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Le opzioni per l'estrazione dei collegamenti ipertestuali. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Una collezione di oggetti [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  se l'estrazione dei collegamenti ipertestuali non è supportata.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Estrae i codici a barre dal documento.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Una collezione di oggetti [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  se l'estrazione dei codici a barre non è supportata.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Estrae i codici a barre dalla pagina del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Una collezione di oggetti [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  se l'estrazione dei codici a barre non è supportata.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Estrae i codici a barre dal documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Le opzioni per l'estrazione dei codici a barre. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Una collezione di oggetti [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  se l'estrazione dei codici a barre non è supportata.\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Estrae i codici a barre dalla pagina del documento usando opzioni di personalizzazione (per impostare l'area rettangolare che contiene i codici a barre).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Le opzioni per l'estrazione dei codici a barre. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Una collezione di oggetti [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  se l'estrazione dei codici a barre non è supportata.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Estrae le tabelle dal documento.

Il seguente esempio mostra come estrarre le tabelle dall'intero documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Le opzioni per l'estrazione delle tabelle. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Una collezione di oggetti [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  se l'estrazione delle tabelle non è supportata.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Estrae le tabelle dal documento, rilevandole automaticamente.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Una collezione di oggetti [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  se l'estrazione delle tabelle non è supportata.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Estrae le tabelle dalla pagina del documento.

Il seguente esempio mostra come estrarre le tabelle dalla pagina del documento:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Le opzioni per l'estrazione delle tabelle. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Una collezione di oggetti [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  se l'estrazione delle tabelle non è supportata.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Estrae le tabelle dalla pagina del documento, rilevandole automaticamente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pageIndex | int | L'indice della pagina basato su zero. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Una collezione di oggetti [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  se l'estrazione delle tabelle non è supportata.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Genera una raccolta di [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s di regolazione per il documento.

Specchio Java del C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (commit d4e691b /
ae9e98c). Utile come modello di partenza che l'utente può poi ridurre o rinominare.

### Algorithm

1. Seleziona la pagina da  options.getPageIndex()  (predefinito  0 ).
2. Se il documento supporta l'estrazione di aree di testo, chiama #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) ed emetti un [TemplateField](../../com.groupdocs.parser.templates/templatefield) per ogni area di testo non vuota, denominata  {prefix}_{n}  (prefisso predefinito  "Field" ). Ogni campo ottiene un [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) nel rettangolo dell'area di testo, con la larghezza della pagina registrata come  pageWidth  così il ridimensionamento successivo del modello funziona.
3. Se il documento non supporta le aree di testo, restituisci  null .

### OCR caveat

L'implementazione C# esegue l'OCR sull'anteprima della pagina per derivare i campi quando il documento è solo immagine. Il [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) di Java è fornito dall'utente, quindi la generazione basata su OCR ha senso solo se un connettore è configurato E il metodo  recognizeTextAreas(...)  del connettore restituisce rettangoli corretti. Quando  options.getOcrOptions()  è impostato e un connettore è disponibile, la pipeline OCR è preferita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Le opzioni di generazione. Possono essere  null  (applicati i valori predefiniti). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Una iterabile di [TemplateItem](../../com.groupdocs.parser.templates/templateitem) generati, o  null  se non supportato da questo formato di documento.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Estrae le informazioni su tutti i fogli di lavoro nel foglio di calcolo.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Una lista di istanze [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) che contiene informazioni su tutti i fogli di lavoro nel foglio di calcolo.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Estrae le informazioni sul foglio di lavoro.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | worksheetIndex | int | L'indice basato su zero del foglio di lavoro. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Estrae le celle del foglio di lavoro.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | worksheetIndex | int | L'indice basato su zero del foglio di lavoro. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Una collezione di istanze [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) che contiene i dati della cella.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Estrae le celle del foglio di lavoro usando opzioni di personalizzazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | worksheetIndex | int | L'indice basato su zero del foglio di lavoro. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Le opzioni di estrazione del foglio di lavoro. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Una collezione di istanze [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) che contiene i dati della cella.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Analizza il documento con il modello generato dall'utente.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Il modello generato dall'utente. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Analizza il documento con il modello generato dall'utente utilizzando le opzioni fornite.

Se
options.getPageIndex()
è impostato, solo quella pagina viene analizzata; altrimenti tutte le pagine vengono analizzate.

Il supporto OCR dipende da [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) configurato in [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Il modello generato dall'utente. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Le opzioni di parse-by-template. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Analizza il documento selezionando automaticamente il modello più adatto da una raccolta.

Specchio di C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
introdotto nel commit 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), e il modello che produce
vince il numero più alto di campi popolati (aree di pagina non nulle con testo non vuoto). L'implementazione C# utilizza
corrispondenza di hidden-marker contro un passaggio OCR; quel percorso non è ancora disponibile in Java perché i marker hidden-field e
il TemplatePageOcrParser guidato da OCR non è stato portato, quindi questo conteggio dei campi popolati è usato come fallback trasparente.
Gli chiamanti che necessitano di un comportamento identico a C# dovrebbero collegare un selettore personalizzato una volta che il motore OCR è configurato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Una raccolta di modelli candidati. Il parser sceglierà quello con la migliore corrispondenza. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Opzioni di parsing. Può essere null. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Analizza il modulo del documento.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Il seguente esempio mostra come analizzare una forma del documento:

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


Estrae un testo strutturato dal documento.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - Un'istanza della classe  org.w3c.dom.Document  con struttura di testo XML; null se l'estrazione della struttura di testo non è supportata.

### close() {#close--}
```
public void close()
```


Chiude questa risorsa, rilasciando eventuali risorse sottostanti.


