---
title: "Parser"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示控制文本图像容器提取和解析功能的主类。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

表示控制文本、图像、容器提取和解析功能的主类。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以从 URL 提取数据。 |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以使用 loadOptions 从 URL 提取数据。 |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以使用 parserSettings 从 URL 提取数据。 |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以使用 loadOptions 和 parserSettings 从 URL 提取数据。 |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以从数据库提取数据。 |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以从数据库提取数据。 |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | 使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | 使用 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 和 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | 使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | 使用 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 和 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | 返回关于文件的一般信息。 |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | 返回关于文件的一般信息。 |
|
|  | [getFeatures()](#getFeatures--) | 获取支持的功能。 |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | 生成文档页面预览。 |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | 使用自定义选项生成文档页面预览。 |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | 获取页面预览。 |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | 返回关于文档的一般信息。 |
|
|  | [getText()](#getText--) | 从文档中提取文本。 |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | 使用文本选项从文档中提取文本页（以启用原始快速文本提取模式）。 |
|
|  | [getText(int pageIndex)](#getText-int-) | 从文档页提取文本。 |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | 使用文本选项从文档页提取文本（以启用原始快速文本提取模式）。 |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | 从文档中提取格式化文本。 |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | 从文档页提取格式化文本。 |
|
|  | [search(String keyword)](#search-java.lang.String-) | 在文档中搜索关键字。 |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | 使用搜索选项（正则表达式、区分大小写等）在文档中搜索关键字。 |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | 从文档中提取高亮。 |
|
|  | [getToc()](#getToc--) | 从文档中提取目录。 |
|
|  | [getMetadata()](#getMetadata--) | 从文档中提取元数据。 |
|
|  | [getAnnotations()](#getAnnotations--) | 从文档中提取批注。 |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | 从文档页提取批注。 |
|
|  | [getContainer()](#getContainer--) | 从文档中提取容器对象，以处理包含附件、ZIP 存档等的格式。 |
|
|  | [getTextAreas()](#getTextAreas--) | 从文档中提取文本区域。 |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | 使用自定义选项（正则表达式、区分大小写等）从文档中提取文本区域。 |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | 从文档页提取文本区域。 |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | 使用自定义选项（正则表达式、区分大小写等）从文档页提取文本区域。 |
|
|  | [getImages()](#getImages--) | 从文档中提取图像。 |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | 使用自定义选项（设置包含图像的矩形区域）从文档中提取图像。 |
|
|  | [getImages(int pageIndex)](#getImages-int-) | 从文档页提取图像。 |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | 使用自定义选项（设置包含图像的矩形区域）从文档页提取图像。 |
|
|  | [getHyperlinks()](#getHyperlinks--) | 从文档中提取超链接。 |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | 从文档页提取超链接。 |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | 使用自定义选项（设置包含超链接的矩形区域）从文档中提取超链接。 |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | 使用自定义选项（设置包含超链接的矩形区域）从文档页提取超链接。 |
|
|  | [getBarcodes()](#getBarcodes--) | 从文档中提取条形码。 |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | 从文档页面中提取条形码。 |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | 使用自定义选项（设置包含条形码的矩形区域）从文档中提取条形码。 |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | 使用自定义选项（设置包含条形码的矩形区域）从文档页面中提取条形码。 |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | 从文档中提取表格。 |
|
|  | [getTables()](#getTables--) | 从文档中提取表格，自动检测它们。 |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | 从文档页面中提取表格。 |
|
|  | [getTables(int pageIndex)](#getTables-int-) | 从文档页面中提取表格，自动检测它们。 |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | 为文档生成一组调整[TemplateItem](../../com.groupdocs.parser.templates/templateitem)。 |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | 提取电子表格中所有工作表的信息。 |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | 提取工作表的信息。 |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | 提取工作表单元格。 |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | 使用自定义选项提取工作表单元格。 |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | 使用用户生成的模板解析文档。 |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | 使用用户生成的模板和提供的选项解析文档。 |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | 通过从集合中自动选择最匹配的模板来解析文档。 |
|
|  | [parseForm()](#parseForm--) | 解析文档表单。 |
|
|  | [getStructure()](#getStructure--) | 从文档中提取结构化文本。 |
|
|  | [close()](#close--) | 关闭此资源，释放所有底层资源。 |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以从 URL 提取数据。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | url | java.net.URL | 请求发送到的 URL |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以使用 loadOptions 从 URL 提取数据。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | url | java.net.URL | 请求发送到的 URL。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开文件的选项。 |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以使用 parserSettings 从 URL 提取数据。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | url | java.net.URL | 请求发送到的 URL。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以使用 loadOptions 和 parserSettings 从 URL 提取数据。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | url | java.net.URL | 请求发送到的 URL。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开文件的选项。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以从数据库提取数据。

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

以下示例展示了如何从 Sqlite 数据库提取数据：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 连接 | java.sql.Connection | 数据库连接。 |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例，以从数据库提取数据。

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

以下示例展示了如何从 Sqlite 数据库提取数据：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 连接 | java.sql.Connection | 数据库连接。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

下面的示例展示了如何从 Exchange Server 提取电子邮件：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | 电子邮件连接。 |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

下面的示例展示了如何从 Exchange Server 提取电子邮件：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | 电子邮件连接。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

下面的示例展示了如何从本地磁盘加载文档：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

文档密码通过 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类传递：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开文件的选项。 |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


使用 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 和 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

下面的示例展示了如何通过 [ILogger](../../com.groupdocs.parser.options/ilogger) 接口获取信息：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开文件的选项。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

下面的示例展示了如何从流加载文档：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

在某些情况下，需要定义 [FileFormat](../../com.groupdocs.parser.options/fileformat)。这适用于特殊情况（数据库、电子邮件服务器）
以及通过内容检测文件类型：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开文件的选项。 |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


使用 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


使用 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 和 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 初始化 [Parser](../../com.groupdocs.parser/parser) 类的新实例。

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

下面的示例展示了如何通过 [ILogger](../../com.groupdocs.parser.options/ilogger) 接口获取信息：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 打开文件的选项。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 用于自定义数据提取的解析器设置。 |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


返回关于文件的一般信息。

下面的代码展示了如何检查文件是否受密码保护：

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


返回关于文件的一般信息。

下面的代码展示了如何检查文件是否受密码保护：

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档 | java.io.InputStream | 源输入流。 |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


获取支持的功能。

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

如果不支持此功能，方法将返回
null
而不是该值。某些操作可能会消耗
大量时间。因此，仅仅检查功能是否受支持而调用此方法并不理想。
为此目的使用 Features 属性：

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


生成文档页面预览。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.io.OutputStream - 包含文档页面图像的 java.io.OutputStream 实例；如果不支持页面预览生成，则为 null。

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


使用自定义选项生成文档页面预览。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | 用于自定义预览生成的选项。 |
|

**Returns:**
java.io.OutputStream - 包含文档页面图像的 java.io.OutputStream 实例；如果不支持页面预览生成，则为 null。

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


获取页面预览。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | 用于设置预览生成的需求和流委托的选项。 |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


返回关于文档的一般信息。

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

下面的示例展示了如何获取文档信息：

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


从文档中提取文本。

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

下面的示例展示了如何从文档中提取文本：

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


使用文本选项从文档中提取文本页（以启用原始快速文本提取模式）。

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

下面的示例展示了如何从文档中提取原始文本：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | 文本提取选项。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


从文档页提取文本。

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

下面的示例展示了如何从文档页面提取文本：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


使用文本选项从文档页提取文本（以启用原始快速文本提取模式）。

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

以下示例展示了如何从文档页面提取原始文本：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | 文本提取选项。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


从文档中提取格式化文本。

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

以下示例展示了如何将文档文本提取为 HTML 文本：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | 格式化文本提取选项。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


从文档页提取格式化文本。

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

以下示例展示了如何将文档页面文本提取为 Markdown 文本：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | 格式化文本提取选项。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


在文档中搜索关键字。

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

以下示例展示了如何在文档中查找关键字：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 关键字 | java.lang.String | 要搜索的关键字。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - 一个 [SearchResult](../../com.groupdocs.parser.data/searchresult) 对象的集合；  null  如果不支持搜索。

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


使用搜索选项（正则表达式、区分大小写等）在文档中搜索关键字。

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

以下示例展示了如何在文档中使用正则表达式进行搜索：

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

以下示例展示了如何在页面上搜索文本：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 关键字 | java.lang.String | 要搜索的关键字。 |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | 搜索选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - 一个 [SearchResult](../../com.groupdocs.parser.data/searchresult) 对象的集合；  null  如果不支持搜索。

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


从文档中提取高亮。

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

以下示例展示了如何提取包含 3 个单词的高亮：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 位置 | int | 高亮的起始位置。 |
|
|  | isDirect | boolean | 指示高亮提取是否直接的值。  true  如果高亮是从位置的右侧提取的；否则，  false 。 |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 高亮提取选项。 |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


从文档中提取目录。

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

以下示例展示了如何从 EPUB 文件提取目录：

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - 一个目录项的集合；  null  如果不支持目录提取。

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


从文档中提取元数据。

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

以下示例展示了如何从文档中提取元数据：

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - 一个元数据项的集合；  null  如果不支持元数据提取。

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


从文档中提取批注。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - 一个注释项的集合；  null  如果不支持注释提取。

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


从文档页提取批注。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - 一个注释项的集合；  null  如果不支持注释提取。

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


从文档中提取容器对象，以处理包含附件、ZIP 存档等的格式。

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

以下示例展示了如何从 zip 实体中提取文本：

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - 一个容器项的集合；  null  如果不支持容器提取。

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


从文档中提取文本区域。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

以下示例展示了如何从整个文档中提取所有文本区域：

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - 一个 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 对象的集合；  null  如果不支持文本区域提取。

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


使用自定义选项（正则表达式、区分大小写等）从文档中提取文本区域。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

以下示例展示了如何从左上角提取仅包含数字的文本区域：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | 文本区域提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - 一个 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 对象的集合；  null  如果不支持文本区域提取。

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


从文档页提取文本区域。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

要从文档页面提取文本区域，请使用以下方法：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - 一个 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 对象的集合；  null  如果不支持文本区域提取。

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


使用自定义选项（正则表达式、区分大小写等）从文档页提取文本区域。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | 文本区域提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - 一个 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 对象的集合；  null  如果不支持文本区域提取。

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


从文档中提取图像。

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

以下示例展示了如何从整个文档中提取所有图像：

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 一个 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 对象的集合；如果不支持图像提取，则为 null。

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


使用自定义选项（设置包含图像的矩形区域）从文档中提取图像。

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

以下示例展示了如何从左上角仅提取图像：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 图像提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 一个 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 对象的集合；如果不支持图像提取，则为 null。

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


从文档页提取图像。

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

要从文档页面提取图像，请使用以下方法：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 一个 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 对象的集合；如果不支持图像提取，则为 null。

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


使用自定义选项（设置包含图像的矩形区域）从文档页提取图像。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 图像提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 一个 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 对象的集合；如果不支持图像提取，则为 null。

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


从文档中提取超链接。

以下示例展示了如何从整个文档中提取所有超链接：

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 一个 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 对象的集合；如果不支持超链接提取，则为 null。

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


从文档页提取超链接。

以下示例展示了如何从文档页面提取超链接：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 一个 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 对象的集合；如果不支持超链接提取，则为 null。

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


使用自定义选项（设置包含超链接的矩形区域）从文档中提取超链接。

以下示例展示了如何从文档页面区域提取超链接：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 超链接提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 一个 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 对象的集合；如果不支持超链接提取，则为 null。

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


使用自定义选项（设置包含超链接的矩形区域）从文档页提取超链接。

以下示例展示了如何使用自定义选项从文档页面区域提取超链接：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 超链接提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 一个 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 对象的集合；如果不支持超链接提取，则为 null。

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


从文档中提取条形码。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 一个 [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 对象的集合；如果不支持条形码提取，则为 null。

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


从文档页面中提取条形码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 一个 [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 对象的集合；如果不支持条形码提取，则为 null。

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


使用自定义选项（设置包含条形码的矩形区域）从文档中提取条形码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | 条形码提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 一个 [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 对象的集合；如果不支持条形码提取，则为 null。\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


使用自定义选项（设置包含条形码的矩形区域）从文档页面中提取条形码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | 条形码提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 一个 [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 对象的集合；如果不支持条形码提取，则为 null。

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


从文档中提取表格。

以下示例展示了如何从整个文档中提取表格：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | 表格提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 一个 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 null。

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


从文档中提取表格，自动检测它们。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 一个 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 null。

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


从文档页面中提取表格。

以下示例展示了如何从文档页面提取表格：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | 表格提取的选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 一个 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 null。

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


从文档页面中提取表格，自动检测它们。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 一个 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 null。

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


为文档生成一组调整[TemplateItem](../../com.groupdocs.parser.templates/templateitem)。

C# 的 Java 镜像
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (提交 d4e691b /
ae9e98c)。此模板可作为起始点，用户随后可以裁剪或重命名。

### Algorithm

1. 从  options.getPageIndex()  中选择页面（默认  0）。
2. 如果文档支持文本区域提取，调用 #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) 并为每个非空文本区域生成一个 [TemplateField](../../com.groupdocs.parser.templates/templatefield)，命名为  {prefix}_{n}  （默认前缀为 "Field"）。每个字段在文本区域的矩形处获取一个 [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)，并将页面宽度记录为  pageWidth  以便后续模板缩放工作。
3. 如果文档不支持文本区域，返回  null 。

### OCR caveat

C# 实现会对页面预览运行 OCR，以在文档仅为图像时推导字段。Java 的 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 由用户提供，因此只有在配置了连接器且连接器的  recognizeTextAreas(...)  返回正确的矩形时，基于 OCR 的生成才有意义。当  options.getOcrOptions()  被设置且连接器可用时，优先使用 OCR 流程。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | 生成选项。可能为  null  （已应用默认值）。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - 生成的 [TemplateItem](../../com.groupdocs.parser.templates/templateitem) 的可迭代集合，如果此文档格式不支持则为  null 。

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


提取电子表格中所有工作表的信息。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - 包含电子表格中所有工作表信息的 [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) 实例列表。

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


提取工作表的信息。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | worksheetIndex | int | 工作表的零基索引。 |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


提取工作表单元格。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | worksheetIndex | int | 工作表的零基索引。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - 包含单元格数据的 [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) 实例集合。

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


使用自定义选项提取工作表单元格。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | worksheetIndex | int | 工作表的零基索引。 |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | 工作表提取选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - 包含单元格数据的 [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) 实例集合。

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


使用用户生成的模板解析文档。

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | 用户生成的模板。 |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


使用用户生成的模板和提供的选项解析文档。

如果
options.getPageIndex()
被设置时，仅解析该页面；否则解析所有页面。

OCR 支持取决于在 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 中配置的 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase)。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | 用户生成的模板。 |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | 按模板解析的选项。 |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


通过从集合中自动选择最匹配的模板来解析文档。

C# 的镜像
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
在提交 71f3f21 中引入。

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions)，以及产生的模板
拥有最高已填充字段数量（非空页面区域且文本非空）的模板获胜。C# 实现使用
针对 OCR 过程的 hidden-marker 匹配；该路径在 Java 中尚不可用，因为 hidden-field 标记和
基于 OCR 的 TemplatePageOcrParser 尚未移植，因此使用此已填充字段计数作为透明回退。
需要 C# 相同行为的调用者应在 OCR 引擎接通后插入自定义选择器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | 候选模板的集合。解析器将挑选最佳匹配的模板。 |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | 解析选项。可能为 null。 |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


解析文档表单。

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

以下示例展示如何解析文档的某种形式：

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


从文档中提取结构化文本。

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - 一个具有 XML 文本结构的 org.w3c.dom.Document 类实例；如果不支持文本结构提取，则为 null。

### close() {#close--}
```
public void close()
```


关闭此资源，释放所有底层资源。


