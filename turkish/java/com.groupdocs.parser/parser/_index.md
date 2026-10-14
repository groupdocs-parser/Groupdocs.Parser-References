---
title: "Ayrıştırıcı"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metin görüntüleri kapsayıcı çıkarma ve ayrıştırma işlevselliğini kontrol eden ana sınıfı temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Metin, görüntü, konteyner çıkarma ve ayrıştırma işlevselliğini kontrol eden ana sınıfı temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır, loadOptions ile. |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır, parserSettings ile. |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır, loadOptions ve parserSettings ile. |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir veritabanından veri çıkarır. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir veritabanından veri çıkarır. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır. |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır. |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır. |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ile başlatır. |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır. |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ve [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır. |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır. |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ile başlatır. |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır. |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ve [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Bir dosya hakkında genel bilgileri döndürür. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Bir dosya hakkında genel bilgileri döndürür. |
|
|  | [getFeatures()](#getFeatures--) | Desteklenen özellikleri alır. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Bir belge sayfası önizlemesi oluşturur. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Özelleştirme seçeneklerini kullanarak bir belge sayfası önizlemesi oluşturur. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Sayfa önizlemelerini al. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Belge hakkında genel bilgileri döndürür. |
|
|  | [getText()](#getText--) | Belgeden metin çıkarır. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Belgeden metin sayfasını metin seçeneklerini kullanarak çıkarır (ham hızlı metin çıkarma modunu etkinleştirmek için). |
|
|  | [getText(int pageIndex)](#getText-int-) | Belge sayfasından metin çıkarır. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Belge sayfasından metin çıkarır, metin seçeneklerini kullanarak (ham hızlı metin çıkarma modunu etkinleştirmek için). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Belgeden biçimlendirilmiş metin çıkarır. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Belge sayfasından biçimlendirilmiş metin çıkarır. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Belgede bir anahtar kelime arar. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Belgede bir anahtar kelimeyi arama seçeneklerini kullanarak arar (düzenli ifade, büyük/küçük harf duyarlılığı vb.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Belgeden vurgulama çıkarır. |
|
|  | [getToc()](#getToc--) | Belgeden bir içindekiler tablosu çıkarır. |
|
|  | [getMetadata()](#getMetadata--) | Belgeden meta verileri çıkarır. |
|
|  | [getAnnotations()](#getAnnotations--) | Belgeden açıklamaları çıkarır. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Belge sayfasından açıklamaları çıkarır. |
|
|  | [getContainer()](#getContainer--) | Ekler, ZIP arşivleri vb. içeren formatlarla çalışmak için belgeden bir konteyner nesnesi çıkarır. |
|
|  | [getTextAreas()](#getTextAreas--) | Belgeden metin alanlarını çıkarır. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Belgeden metin alanlarını özelleştirme seçeneklerini (düzenli ifade, büyük/küçük harf duyarlılığı vb.) kullanarak çıkarır. |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Belge sayfasından metin alanlarını çıkarır. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Belge sayfasından metin alanlarını özelleştirme seçeneklerini (düzenli ifade, büyük/küçük harf duyarlılığı vb.) kullanarak çıkarır. |
|
|  | [getImages()](#getImages--) | Belgeden görüntüleri çıkarır. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Belgeden görüntüleri, görüntüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır. |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Belge sayfasından görüntüleri çıkarır. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Belge sayfasından görüntüleri, görüntüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır. |
|
|  | [getHyperlinks()](#getHyperlinks--) | Belgeden köprüleri çıkarır. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Belge sayfasından köprüleri çıkarır. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Belgeden köprüleri, köprüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır. |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Belge sayfasından köprüleri, köprüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır. |
|
|  | [getBarcodes()](#getBarcodes--) | Belgeden barkodları çıkarır. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Belge sayfasından barkodları çıkarır. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Belgeden barkodları, barkodları içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır. |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Belge sayfasından barkodları, barkodları içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır. |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Belgeden tabloları çıkarır. |
|
|  | [getTables()](#getTables--) | Belgeden tabloları otomatik olarak tespit ederek çıkarır. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Belge sayfasından tabloları çıkarır. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Belge sayfasından tabloları otomatik olarak tespit ederek çıkarır. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Belge için düzeltme [TemplateItem](../../com.groupdocs.parser.templates/templateitem) öğelerinin bir koleksiyonunu oluşturur. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Elektronik tablodaki tüm çalışma sayfalarıyla ilgili bilgileri çıkarır. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Çalışma sayfasıyla ilgili bilgileri çıkarır. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Çalışma sayfası hücrelerini çıkarır. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Özelleştirme seçeneklerini kullanarak çalışma sayfası hücrelerini çıkarır. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Kullanıcı tarafından oluşturulan şablonla belgeyi ayrıştırır. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Sağlanan seçeneklerle kullanıcı tarafından oluşturulan şablonla belgeyi ayrıştırır. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Belgeyi, bir koleksiyondan en uygun şablonu otomatik olarak seçerek ayrıştırır. |
|
|  | [parseForm()](#parseForm--) | Belge formunu ayrıştırır. |
|
|  | [getStructure()](#getStructure--) | Belgeden yapılandırılmış bir metin çıkarır. |
|
|  | [close()](#close--) | Bu kaynağı kapatır, altındaki tüm kaynakları serbest bırakır. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | url | java.net.URL | İsteğin gönderildiği URL |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır, loadOptions ile.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | url | java.net.URL | İsteğin gönderildiği URL. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Dosyayı açmak için seçenekler. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır, parserSettings ile.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | url | java.net.URL | İsteğin gönderildiği URL. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir URL'den veri çıkarır, loadOptions ve parserSettings ile.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | url | java.net.URL | İsteğin gönderildiği URL. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Dosyayı açmak için seçenekler. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir veritabanından veri çıkarır.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Aşağıdaki örnek, Sqlite veritabanından veri nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | bağlantı | java.sql.Connection | Veritabanı bağlantısı. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır ve bir veritabanından veri çıkarır.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Aşağıdaki örnek, Sqlite veritabanından veri nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | bağlantı | java.sql.Connection | Veritabanı bağlantısı. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Aşağıdaki örnek, Exchange Server'dan e-posta nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | E-posta bağlantısı. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Aşağıdaki örnek, Exchange Server'dan e-posta nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | E-posta bağlantısı. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Aşağıdaki örnek, belgeyi yerel diskten nasıl yükleyeceğinizi gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ile başlatır.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Belge parolası, [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı tarafından iletilir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Dosyayı açmak için seçenekler. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ve [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Aşağıdaki örnek, bilgiyi [ILogger](../../com.groupdocs.parser.options/ilogger) arayüzü aracılığıyla nasıl alacağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Dosyayı açmak için seçenekler. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini başlatır.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Aşağıdaki örnek, belgeyi akıştan nasıl yükleyeceğinizi gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ile başlatır.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Bazı durumlarda [FileFormat](../../com.groupdocs.parser.options/fileformat) tanımlamak gerekir. Hem özel durumlar (veritabanları, e-posta sunucusu) için
ve içeriğe göre dosya türlerini tespit etmek için:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Dosyayı açmak için seçenekler. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Yeni bir [Parser](../../com.groupdocs.parser/parser) sınıfının örneğini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ve [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile başlatır.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Aşağıdaki örnek, bilgiyi [ILogger](../../com.groupdocs.parser.options/ilogger) arayüzü aracılığıyla nasıl alacağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Dosyayı açmak için seçenekler. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Bir dosya hakkında genel bilgileri döndürür.

Aşağıdaki kod, bir dosyanın şifre korumalı olup olmadığını nasıl kontrol edeceğinizi gösterir:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Bir dosya hakkında genel bilgileri döndürür.

Aşağıdaki kod, bir dosyanın şifre korumalı olup olmadığını nasıl kontrol edeceğinizi gösterir:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | belge | java.io.InputStream | Kaynak giriş akışı. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Desteklenen özellikleri alır.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Özellik desteklenmiyorsa, yöntem döndürür
null
değer yerine. Bazı işlemler tüketebilir
önemli miktarda zaman. Bu nedenle, yalnızca özelliğin desteklenip desteklenmediğini kontrol etmek için yöntemi çağırmak optimal değildir.
Bu amaçla Features özelliği kullanılır:

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


Bir belge sayfası önizlemesi oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.io.OutputStream - Belge sayfasının görüntüsünü içeren bir java.io.OutputStream örneği; sayfa önizlemesi oluşturulması desteklenmiyorsa  null

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Özelleştirme seçeneklerini kullanarak bir belge sayfası önizlemesi oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Önizleme oluşturmayı özelleştirmek için seçenekler. |
|

**Returns:**
java.io.OutputStream - Belge sayfasının görüntüsünü içeren bir java.io.OutputStream örneği; sayfa önizlemesi oluşturulması desteklenmiyorsa  null

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Sayfa önizlemelerini al.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlamak için seçenekler. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Belge hakkında genel bilgileri döndürür.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

Aşağıdaki örnek, belge bilgilerini nasıl alacağınızı gösterir:

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


Belgeden metin çıkarır.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Aşağıdaki örnek, bir belgeden metin nasıl çıkarılacağını gösterir:

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


Belgeden metin sayfasını metin seçeneklerini kullanarak çıkarır (ham hızlı metin çıkarma modunu etkinleştirmek için).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Aşağıdaki örnek, bir belgeden ham metin nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Metin çıkarma seçenekleri. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Belge sayfasından metin çıkarır.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Aşağıdaki örnek, belge sayfasından metin nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Belge sayfasından metin çıkarır, metin seçeneklerini kullanarak (ham hızlı metin çıkarma modunu etkinleştirmek için).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

Aşağıdaki örnek, belge sayfasından ham metin nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Metin çıkarma seçenekleri. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Belgeden biçimlendirilmiş metin çıkarır.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Aşağıdaki örnek, belge metnini HTML metni olarak nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Biçimlendirilmiş metin çıkarma seçenekleri. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Belge sayfasından biçimlendirilmiş metin çıkarır.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

Aşağıdaki örnek, belge sayfası metnini Markdown metni olarak nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Biçimlendirilmiş metin çıkarma seçenekleri. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Belgede bir anahtar kelime arar.

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

Aşağıdaki örnek, bir belgede anahtar kelimeyi nasıl bulacağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | anahtar kelime | java.lang.String | Aranacak anahtar kelime. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) nesnelerinin bir koleksiyonu; arama desteklenmiyorsa  null

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Belgede bir anahtar kelimeyi arama seçeneklerini kullanarak arar (düzenli ifade, büyük/küçük harf duyarlılığı vb.).

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

Aşağıdaki örnek, bir belgede düzenli ifade kullanarak nasıl arama yapılacağını gösterir:

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

Aşağıdaki örnek, sayfalarda bir metni nasıl arayacağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | anahtar kelime | java.lang.String | Aranacak anahtar kelime. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Arama seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) nesnelerinin bir koleksiyonu; arama desteklenmiyorsa  null

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Belgeden vurgulama çıkarır.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

Aşağıdaki örnek, 3 kelime içeren bir vurguyu nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | konum | int | Vurgunun başlangıç konumu. |
|
|  | isDirect | boolean | Vurgunun çıkarılmasının doğrudan olup olmadığını gösteren değer.  true  eğer vurgulama konumun sağından çıkarıldıysa; aksi takdirde,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Vurgulama çıkarma seçenekleri. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Belgeden bir içindekiler tablosu çıkarır.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

Aşağıdaki örnek, EPUB dosyasından içindekiler tablosunun nasıl çıkarılacağını gösterir:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - İçindekiler öğelerinin bir koleksiyonu;  null  eğer içindekiler çıkarımı desteklenmiyorsa.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Belgeden meta verileri çıkarır.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

Aşağıdaki örnek, bir belgeden meta verilerin nasıl çıkarılacağını gösterir:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Meta veri öğelerinin bir koleksiyonu;  null  eğer meta veri çıkarımı desteklenmiyorsa.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Belgeden açıklamaları çıkarır.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Açıklama öğelerinin bir koleksiyonu;  null  eğer açıklama çıkarımı desteklenmiyorsa.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Belge sayfasından açıklamaları çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Açıklama öğelerinin bir koleksiyonu;  null  eğer açıklama çıkarımı desteklenmiyorsa.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Ekler, ZIP arşivleri vb. içeren formatlarla çalışmak için belgeden bir konteyner nesnesi çıkarır.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

Aşağıdaki örnek, zip varlıklarından bir metnin nasıl çıkarılacağını gösterir:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Kapsayıcı öğelerinin bir koleksiyonu;  null  eğer kapsayıcı çıkarımı desteklenmiyorsa.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Belgeden metin alanlarını çıkarır.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Aşağıdaki örnek, tüm belgede bulunan tüm metin alanlarının nasıl çıkarılacağını gösterir:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) nesnelerinin bir koleksiyonu;  null  eğer metin alanları çıkarımı desteklenmiyorsa.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Belgeden metin alanlarını özelleştirme seçeneklerini (düzenli ifade, büyük/küçük harf duyarlılığı vb.) kullanarak çıkarır.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Aşağıdaki örnek, üst sol köşeden sadece rakam içeren metin alanlarının nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Metin alanı çıkarma seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) nesnelerinin bir koleksiyonu;  null  eğer metin alanları çıkarımı desteklenmiyorsa.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Belge sayfasından metin alanlarını çıkarır.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Bir belge sayfasından metin alanlarını çıkarmak için aşağıdaki yöntem kullanılır:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) nesnelerinin bir koleksiyonu;  null  eğer metin alanları çıkarımı desteklenmiyorsa.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Belge sayfasından metin alanlarını özelleştirme seçeneklerini (düzenli ifade, büyük/küçük harf duyarlılığı vb.) kullanarak çıkarır.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Metin alanı çıkarma seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) nesnelerinin bir koleksiyonu;  null  eğer metin alanları çıkarımı desteklenmiyorsa.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Belgeden görüntüleri çıkarır.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Aşağıdaki örnek, tüm belgede bulunan tüm görüntülerin nasıl çıkarılacağını gösterir:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) nesnelerinin bir koleksiyonu;  null  eğer görüntü çıkarımı desteklenmiyorsa.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Belgeden görüntüleri, görüntüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Aşağıdaki örnek, üst sol köşeden sadece görüntülerin nasıl çıkarılacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Görüntü çıkarma seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) nesnelerinin bir koleksiyonu;  null  eğer görüntü çıkarımı desteklenmiyorsa.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Belge sayfasından görüntüleri çıkarır.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Bir belge sayfasından görüntüleri çıkarmak için aşağıdaki yöntem kullanılır:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) nesnelerinin bir koleksiyonu;  null  eğer görüntü çıkarımı desteklenmiyorsa.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Belge sayfasından görüntüleri, görüntüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Görüntü çıkarma seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) nesnelerinin bir koleksiyonu;  null  eğer görüntü çıkarımı desteklenmiyorsa.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Belgeden köprüleri çıkarır.

Aşağıdaki örnek, tüm belgeden tüm hiperlinkleri nasıl çıkaracağınızı gösterir:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea] nesnelerinin bir koleksiyonu;  null  eğer hiperlink çıkarımı desteklenmiyorsa.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Belge sayfasından köprüleri çıkarır.

Aşağıdaki örnek, belge sayfasından hiperlinkleri nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea] nesnelerinin bir koleksiyonu;  null  eğer hiperlink çıkarımı desteklenmiyorsa.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Belgeden köprüleri, köprüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır.

Aşağıdaki örnek, belge sayfa alanından hiperlinkleri nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Hiperlink çıkarımı için seçenekler. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea] nesnelerinin bir koleksiyonu;  null  eğer hiperlink çıkarımı desteklenmiyorsa.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Belge sayfasından köprüleri, köprüleri içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır.

Aşağıdaki örnek, özelleştirme seçeneklerini kullanarak belge sayfa alanından hiperlinkleri nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Hiperlink çıkarımı için seçenekler. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea] nesnelerinin bir koleksiyonu;  null  eğer hiperlink çıkarımı desteklenmiyorsa.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Belgeden barkodları çıkarır.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea] nesnelerinin bir koleksiyonu;  null  eğer barkod çıkarımı desteklenmiyorsa.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Belge sayfasından barkodları çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea] nesnelerinin bir koleksiyonu;  null  eğer barkod çıkarımı desteklenmiyorsa.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Belgeden barkodları, barkodları içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Barkod çıkarımı için seçenekler. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea] nesnelerinin bir koleksiyonu;  null  eğer barkod çıkarımı desteklenmiyorsa.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Belge sayfasından barkodları, barkodları içeren dikdörtgen alanı ayarlamak için özelleştirme seçeneklerini kullanarak çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Barkod çıkarımı için seçenekler. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea] nesnelerinin bir koleksiyonu;  null  eğer barkod çıkarımı desteklenmiyorsa.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Belgeden tabloları çıkarır.

Aşağıdaki örnek, tüm belgeden tabloları nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Tablo çıkarımı için seçenekler. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea] nesnelerinin bir koleksiyonu;  null  eğer tablo çıkarımı desteklenmiyorsa.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Belgeden tabloları otomatik olarak tespit ederek çıkarır.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea] nesnelerinin bir koleksiyonu;  null  eğer tablo çıkarımı desteklenmiyorsa.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Belge sayfasından tabloları çıkarır.

Aşağıdaki örnek, belge sayfasından tabloları nasıl çıkaracağınızı gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Tablo çıkarımı için seçenekler. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea] nesnelerinin bir koleksiyonu;  null  eğer tablo çıkarımı desteklenmiyorsa.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Belge sayfasından tabloları otomatik olarak tespit ederek çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea] nesnelerinin bir koleksiyonu;  null  eğer tablo çıkarımı desteklenmiyorsa.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Belge için düzeltme [TemplateItem](../../com.groupdocs.parser.templates/templateitem) öğelerinin bir koleksiyonunu oluşturur.

C#'ın Java aynası
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (commits d4e691b /
ae9e98c). Kullanıcı tarafından daha sonra kırpılabilecek veya yeniden adlandırılabilecek bir başlangıç şablonu olarak kullanışlı.

### Algorithm

1. Sayfayı  options.getPageIndex()  üzerinden seçin (varsayılan  0 ).
2. Eğer belge metin-alanı çıkarımını destekliyorsa, #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) metodunu çağırın ve boş olmayan her metin alanı için bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) oluşturun, {prefix}_{n} adıyla (varsayılan önek "Field"). Her alan, metin alanının dikdörtgeninde bir [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) alır; sayfanın genişliği pageWidth olarak kaydedilir, böylece sonraki şablon ölçeklendirmesi çalışır.
3. Eğer belge metin alanlarını desteklemiyorsa,  null  döndürün.

### OCR caveat

C# uygulaması, belge yalnızca görüntü olduğunda alanları türetmek için sayfa önizlemesi üzerinde OCR çalıştırır. Java'nın [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) kullanıcı tarafından sağlanır, bu yüzden OCR tabanlı oluşturma yalnızca bir bağlayıcı yapılandırılmış ve bağlayıcının  recognizeTextAreas(...)  doğru dikdörtgenler döndürdüğü durumlarda anlamlıdır.  options.getOcrOptions()  ayarlandığında ve bir bağlayıcı mevcut olduğunda, OCR işlem hattı tercih edilir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Oluşturma seçenekleri.  null  olabilir (varsayılanlar uygulanır). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Oluşturulan [TemplateItem](../../com.groupdocs.parser.templates/templateitem) öğelerinin bir iterable'ı, veya bu belge formatı tarafından desteklenmiyorsa  null .

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Elektronik tablodaki tüm çalışma sayfalarıyla ilgili bilgileri çıkarır.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Elektronik tablo içinde bulunan tüm çalışma sayfaları hakkında bilgi içeren [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) örneklerinin bir listesi.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Çalışma sayfasıyla ilgili bilgileri çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | worksheetIndex | int | Çalışma sayfasının sıfır tabanlı dizini. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Çalışma sayfası hücrelerini çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | worksheetIndex | int | Çalışma sayfasının sıfır tabanlı dizini. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Hücre verilerini içeren [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) örneklerinden oluşan bir koleksiyon.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Özelleştirme seçeneklerini kullanarak çalışma sayfası hücrelerini çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | worksheetIndex | int | Çalışma sayfasının sıfır tabanlı dizini. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Çalışma sayfası çıkarma seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Hücre verilerini içeren [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) örneklerinden oluşan bir koleksiyon.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Kullanıcı tarafından oluşturulan şablonla belgeyi ayrıştırır.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Kullanıcı tarafından oluşturulan şablon. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Sağlanan seçeneklerle kullanıcı tarafından oluşturulan şablonla belgeyi ayrıştırır.

Eğer
options.getPageIndex()
ayarlanmışsa, yalnızca o sayfa ayrıştırılır; aksi takdirde tüm sayfalar ayrıştırılır.

OCR desteği, [ParserSettings](../../com.groupdocs.parser.options/parsersettings) içinde yapılandırılan [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) öğesine bağlıdır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Kullanıcı tarafından oluşturulan şablon. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Şablona göre ayrıştırma seçenekleri. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Belgeyi, bir koleksiyondan en uygun şablonu otomatik olarak seçerek ayrıştırır.

C#'ın aynası
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
commit 71f3f21'de tanıtıldı.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), ve üreten şablon
en yüksek sayıda doldurulmuş alan (boş olmayan metin içeren null olmayan sayfa bölgeleri) kazanır. C# uygulaması şunu kullanır
gizli-işaretçi eşleştirmesi bir OCR geçişine karşı; bu yol Java'da henüz mevcut değil çünkü gizli-alan işaretçileri ve
OCR tabanlı TemplatePageOcrParser taşınmadığı için, bu doldurulmuş alan sayısı şeffaf bir geri dönüş olarak kullanılır.
C# ile aynı davranışı gerektiren çağırıcılar, OCR motoru bağlandığında özel bir seçici eklemelidir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Aday şablonlardan oluşan bir koleksiyon. Ayrıştırıcı en iyi eşleşeni seçecek. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Ayrıştırma seçenekleri. Null olabilir. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Belge formunu ayrıştırır.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Aşağıdaki örnek, belgenin bir formunu nasıl ayrıştıracağınızı gösterir:

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


Belgeden yapılandırılmış bir metin çıkarır.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - XML metin yapısına sahip  org.w3c.dom.Document  sınıfının bir örneği; metin yapısı çıkarımı desteklenmiyorsa  null  olur.

### close() {#close--}
```
public void close()
```


Bu kaynağı kapatır, altındaki tüm kaynakları serbest bırakır.


