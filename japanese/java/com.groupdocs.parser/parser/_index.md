---
title: "Parser"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テキスト画像コンテナの抽出と解析機能を制御するメインクラスを表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

テキスト、画像、コンテナの抽出および解析機能を制御するメインクラスを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | loadOptions を使用して URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | parserSettings を使用して URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | loadOptions と parserSettings を使用して URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | データベースからデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | データベースからデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | 新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | 新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | 新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) を使用して、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | 新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。 |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。 |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | 新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) を使用して、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。 |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | 新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。 |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | 新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | ファイルに関する一般情報を返します。 |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | ファイルに関する一般情報を返します。 |
|
|  | [getFeatures()](#getFeatures--) | サポートされている機能を取得します。 |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | ドキュメントページのプレビューを生成します。 |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | カスタマイズオプションを使用してドキュメントページのプレビューを生成します。 |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | ページのプレビューを取得します。 |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | ドキュメントに関する一般情報を返します。 |
|
|  | [getText()](#getText--) | ドキュメントからテキストを抽出します。 |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | テキストオプションを使用してドキュメントからテキストページを抽出します（生の高速テキスト抽出モードを有効にするため）。 |
|
|  | [getText(int pageIndex)](#getText-int-) | ドキュメントページからテキストを抽出します。 |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | テキストオプションを使用してドキュメントページからテキストを抽出します（生の高速テキスト抽出モードを有効にするため）。 |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | ドキュメントから書式付きテキストを抽出します。 |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | ドキュメントページから書式付きテキストを抽出します。 |
|
|  | [search(String keyword)](#search-java.lang.String-) | ドキュメント内のキーワードを検索します。 |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | 検索オプション（正規表現、大小文字の区別など）を使用してドキュメント内のキーワードを検索します。 |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | ドキュメントからハイライトを抽出します。 |
|
|  | [getToc()](#getToc--) | ドキュメントから目次を抽出します。 |
|
|  | [getMetadata()](#getMetadata--) | ドキュメントからメタデータを抽出します。 |
|
|  | [getAnnotations()](#getAnnotations--) | ドキュメントから注釈を抽出します。 |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | ドキュメントページから注釈を抽出します。 |
|
|  | [getContainer()](#getContainer--) | 添付ファイルやZIPアーカイブなどを含む形式を扱うために、ドキュメントからコンテナオブジェクトを抽出します。 |
|
|  | [getTextAreas()](#getTextAreas--) | ドキュメントからテキスト領域を抽出します。 |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | カスタマイズオプション（正規表現、大小文字の区別など）を使用してドキュメントからテキスト領域を抽出します。 |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | ドキュメントページからテキスト領域を抽出します。 |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | カスタマイズオプション（正規表現、大小文字の区別など）を使用して、ドキュメントページからテキスト領域を抽出します。 |
|
|  | [getImages()](#getImages--) | ドキュメントから画像を抽出します。 |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | カスタマイズオプション（画像が含まれる矩形領域を設定）を使用して、ドキュメントから画像を抽出します。 |
|
|  | [getImages(int pageIndex)](#getImages-int-) | ドキュメントページから画像を抽出します。 |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | カスタマイズオプション（画像が含まれる矩形領域を設定）を使用して、ドキュメントページから画像を抽出します。 |
|
|  | [getHyperlinks()](#getHyperlinks--) | ドキュメントからハイパーリンクを抽出します。 |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | ドキュメントページからハイパーリンクを抽出します。 |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | カスタマイズオプション（ハイパーリンクが含まれる矩形領域を設定）を使用して、ドキュメントからハイパーリンクを抽出します。 |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | カスタマイズオプション（ハイパーリンクが含まれる矩形領域を設定）を使用して、ドキュメントページからハイパーリンクを抽出します。 |
|
|  | [getBarcodes()](#getBarcodes--) | ドキュメントからバーコードを抽出します。 |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | ドキュメントページからバーコードを抽出します。 |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | カスタマイズオプション（バーコードが含まれる矩形領域を設定）を使用して、ドキュメントからバーコードを抽出します。 |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | カスタマイズオプション（バーコードが含まれる矩形領域を設定）を使用して、ドキュメントページからバーコードを抽出します。 |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | ドキュメントからテーブルを抽出します。 |
|
|  | [getTables()](#getTables--) | ドキュメントからテーブルを抽出し、自動的に検出します。 |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | ドキュメントページからテーブルを抽出します。 |
|
|  | [getTables(int pageIndex)](#getTables-int-) | ドキュメントページからテーブルを抽出し、自動的に検出します。 |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | ドキュメント用に調整用の[TemplateItem](../../com.groupdocs.parser.templates/templateitem)コレクションを生成します。 |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | スプレッドシート内のすべてのワークシートに関する情報を抽出します。 |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | ワークシートに関する情報を抽出します。 |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | ワークシートのセルを抽出します。 |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | カスタマイズオプションを使用して、ワークシートのセルを抽出します。 |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | ユーザー生成テンプレートでドキュメントを解析します。 |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | 提供されたオプションを使用して、ユーザー生成テンプレートでドキュメントを解析します。 |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | コレクションから最適なテンプレートを自動的に選択してドキュメントを解析します。 |
|
|  | [parseForm()](#parseForm--) | ドキュメントフォームを解析します。 |
|
|  | [getStructure()](#getStructure--) | ドキュメントから構造化テキストを抽出します。 |
|
|  | [close()](#close--) | このリソースを閉じ、基になるリソースをすべて解放します。 |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | url | java.net.URL | リクエストが送信される URL |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


loadOptions を使用して URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | url | java.net.URL | リクエストが送信される URL。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | ファイルを開くためのオプション。 |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


parserSettings を使用して URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | url | java.net.URL | リクエストが送信される URL。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


loadOptions と parserSettings を使用して URL からデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | url | java.net.URL | リクエストが送信される URL。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | ファイルを開くためのオプション。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


データベースからデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

次の例は、SQLite データベースからデータを抽出する方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 接続 | java.sql.Connection | データベース接続。 |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


データベースからデータを抽出するために、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

次の例は、SQLite データベースからデータを抽出する方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 接続 | java.sql.Connection | データベース接続。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

次の例は、Exchange Server からメールを抽出する方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | メール接続。 |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

次の例は、Exchange Server からメールを抽出する方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | メール接続。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

次の例は、ローカルディスクからドキュメントをロードする方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) を使用して、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

ドキュメントのパスワードは、[LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスによって渡されます。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | ファイルを開くためのオプション。 |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

次の例は、[ILogger](../../com.groupdocs.parser.options/ilogger) インターフェイスを介して情報を取得する方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | ファイルを開くためのオプション。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

次の例は、ストリームからドキュメントをロードする方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) を使用して、新しい [Parser](../../com.groupdocs.parser/parser) クラスのインスタンスを初期化します。

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

場合によっては、[FileFormat](../../com.groupdocs.parser.options/fileformat) を定義する必要があります。特別なケース（データベース、メールサーバー）にも対応します。
そして、コンテンツによってファイルタイプを検出するために：

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | ファイルを開くためのオプション。 |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


新しいインスタンスの [Parser](../../com.groupdocs.parser/parser) クラスを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と [ParserSettings](../../com.groupdocs.parser.options/parsersettings) で初期化します。

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

次の例は、[ILogger](../../com.groupdocs.parser.options/ilogger) インターフェイスを介して情報を取得する方法を示しています。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | ファイルを開くためのオプション。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


ファイルに関する一般情報を返します。

次のコードは、ファイルがパスワードで保護されているかどうかを確認する方法を示しています。

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルへのパスです。 |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


ファイルに関する一般情報を返します。

次のコードは、ファイルがパスワードで保護されているかどうかを確認する方法を示しています。

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ドキュメント | java.io.InputStream | ソース入力ストリーム。 |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


サポートされている機能を取得します。

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

機能がサポートされていない場合、メソッドは返します
null
値の代わりに。いくつかの操作は消費する可能性があります
多くの時間がかかります。そのため、機能のサポートを確認するだけのためにメソッドを呼び出すのは最適ではありません。
この目的のために Features プロパティが使用されます:

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


ドキュメントページのプレビューを生成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.io.OutputStream - ドキュメントページの画像を含む java.io.OutputStream のインスタンスです。ページプレビュー生成がサポートされていない場合は null です。

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


カスタマイズオプションを使用してドキュメントページのプレビューを生成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | プレビュー生成をカスタマイズするためのオプションです。 |
|

**Returns:**
java.io.OutputStream - ドキュメントページの画像を含む java.io.OutputStream のインスタンスです。ページプレビュー生成がサポートされていない場合は null です。

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


ページのプレビューを取得します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | プレビュー生成の要件とストリーム デリゲートを設定するためのオプションです。 |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


ドキュメントに関する一般情報を返します。

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

次の例は、ドキュメント情報を取得する方法を示しています:

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


ドキュメントからテキストを抽出します。

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

次の例は、ドキュメントからテキストを抽出する方法を示しています:

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


テキストオプションを使用してドキュメントからテキストページを抽出します（生の高速テキスト抽出モードを有効にするため）。

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

次の例は、ドキュメントから生テキストを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | テキスト抽出オプションです。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


ドキュメントページからテキストを抽出します。

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

次の例は、ドキュメントページからテキストを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


テキストオプションを使用してドキュメントページからテキストを抽出します（生の高速テキスト抽出モードを有効にするため）。

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

次の例は、ドキュメントページから生テキストを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | テキスト抽出オプションです。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


ドキュメントから書式付きテキストを抽出します。

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

次の例は、ドキュメントテキストを HTML テキストとして抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | 書式付きテキスト抽出オプションです。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


ドキュメントページから書式付きテキストを抽出します。

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

次の例は、ドキュメントページのテキストを Markdown テキストとして抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | 書式付きテキスト抽出オプションです。 |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


ドキュメント内のキーワードを検索します。

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

次の例は、ドキュメント内でキーワードを検索する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | キーワード | java.lang.String | 検索対象のキーワードです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) オブジェクトのコレクションです。検索がサポートされていない場合は null です。

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


検索オプション（正規表現、大小文字の区別など）を使用してドキュメント内のキーワードを検索します。

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

次の例は、ドキュメント内で正規表現を使用して検索する方法を示しています:

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

次の例は、ページ上でテキストを検索する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | キーワード | java.lang.String | 検索対象のキーワードです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | 検索オプションです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) オブジェクトのコレクションです。検索がサポートされていない場合は null です。

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


ドキュメントからハイライトを抽出します。

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

次の例は、3語を含むハイライトを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 位置 | int | ハイライトの開始位置です。 |
|
|  | isDirect | boolean | ハイライト抽出が直接かどうかを示す値です。位置の右側からハイライトが抽出される場合は true、そうでない場合は false です。 |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | ハイライト抽出オプションです。 |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


ドキュメントから目次を抽出します。

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

次の例は、EPUB ファイルから目次を抽出する方法を示しています:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - 目次項目のコレクション; テーブル オブ コンテンツ抽出がサポートされていない場合は null。

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


ドキュメントからメタデータを抽出します。

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

次の例は、ドキュメントからメタデータを抽出する方法を示しています:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - メタデータ項目のコレクション; メタデータ抽出がサポートされていない場合は null。

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


ドキュメントから注釈を抽出します。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - アノテーション項目のコレクション; アノテーション抽出がサポートされていない場合は null。

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


ドキュメントページから注釈を抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - アノテーション項目のコレクション; アノテーション抽出がサポートされていない場合は null。

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


添付ファイルやZIPアーカイブなどを含む形式を扱うために、ドキュメントからコンテナオブジェクトを抽出します。

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

次の例は、ZIP エンティティからテキストを抽出する方法を示しています:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - コンテナ項目のコレクション; コンテナ抽出がサポートされていない場合は null。

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


ドキュメントからテキスト領域を抽出します。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

次の例は、ドキュメント全体からすべてのテキスト領域を抽出する方法を示しています:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) オブジェクトのコレクション; テキスト領域の抽出がサポートされていない場合は null。

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


カスタマイズオプション（正規表現、大小文字の区別など）を使用してドキュメントからテキスト領域を抽出します。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

次の例は、左上隅から数字を含むテキスト領域のみを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | テキスト領域抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) オブジェクトのコレクション; テキスト領域の抽出がサポートされていない場合は null。

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


ドキュメントページからテキスト領域を抽出します。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

ドキュメントページからテキスト領域を抽出するには、次のメソッドを使用します:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) オブジェクトのコレクション; テキスト領域の抽出がサポートされていない場合は null。

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


カスタマイズオプション（正規表現、大小文字の区別など）を使用して、ドキュメントページからテキスト領域を抽出します。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | テキスト領域抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) オブジェクトのコレクション; テキスト領域の抽出がサポートされていない場合は null。

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


ドキュメントから画像を抽出します。

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

次の例は、ドキュメント全体からすべての画像を抽出する方法を示しています:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) オブジェクトのコレクション; 画像の抽出がサポートされていない場合は null。

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


カスタマイズオプション（画像が含まれる矩形領域を設定）を使用して、ドキュメントから画像を抽出します。

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

次の例は、左上隅から画像のみを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 画像抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) オブジェクトのコレクション; 画像の抽出がサポートされていない場合は null。

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


ドキュメントページから画像を抽出します。

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

ドキュメントページから画像を抽出するには、次のメソッドを使用します:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) オブジェクトのコレクション; 画像の抽出がサポートされていない場合は null。

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


カスタマイズオプション（画像が含まれる矩形領域を設定）を使用して、ドキュメントページから画像を抽出します。

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 画像抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) オブジェクトのコレクション; 画像の抽出がサポートされていない場合は null。

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


ドキュメントからハイパーリンクを抽出します。

次の例は、ドキュメント全体からすべてのハイパーリンクを抽出する方法を示しています:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション; ハイパーリンクの抽出がサポートされていない場合は null。

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


ドキュメントページからハイパーリンクを抽出します。

次の例は、ドキュメントページからハイパーリンクを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション; ハイパーリンクの抽出がサポートされていない場合は null。

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


カスタマイズオプション（ハイパーリンクが含まれる矩形領域を設定）を使用して、ドキュメントからハイパーリンクを抽出します。

次の例は、ドキュメントページ領域からハイパーリンクを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | ハイパーリンク抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション; ハイパーリンクの抽出がサポートされていない場合は null。

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


カスタマイズオプション（ハイパーリンクが含まれる矩形領域を設定）を使用して、ドキュメントページからハイパーリンクを抽出します。

次の例は、カスタマイズオプションを使用してドキュメントページ領域からハイパーリンクを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | ハイパーリンク抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション; ハイパーリンクの抽出がサポートされていない場合は null。

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


ドキュメントからバーコードを抽出します。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコードの抽出がサポートされていない場合は null。

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


ドキュメントページからバーコードを抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコードの抽出がサポートされていない場合は null。

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


カスタマイズオプション（バーコードが含まれる矩形領域を設定）を使用して、ドキュメントからバーコードを抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | バーコード抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクションです。バーコード抽出がサポートされていない場合は null です。\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


カスタマイズオプション（バーコードが含まれる矩形領域を設定）を使用して、ドキュメントページからバーコードを抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | バーコード抽出のオプション。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコードの抽出がサポートされていない場合は null。

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


ドキュメントからテーブルを抽出します。

次の例は、ドキュメント全体からテーブルを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | テーブル抽出のオプションです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。テーブル抽出がサポートされていない場合は null です。

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


ドキュメントからテーブルを抽出し、自動的に検出します。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。テーブル抽出がサポートされていない場合は null です。

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


ドキュメントページからテーブルを抽出します。

次の例は、ドキュメントページからテーブルを抽出する方法を示しています:

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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | テーブル抽出のオプションです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。テーブル抽出がサポートされていない場合は null です。

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


ドキュメントページからテーブルを抽出し、自動的に検出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。テーブル抽出がサポートされていない場合は null です。

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


ドキュメント用に調整用の[TemplateItem](../../com.groupdocs.parser.templates/templateitem)コレクションを生成します。

C# の Java ミラーです。
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (コミット d4e691b /
ae9e98c)。ユーザーが後でトリミングまたは名前変更できる開始テンプレートとして便利です。

### Algorithm

1. options.getPageIndex() からページを選択します（デフォルトは 0）。
2. ドキュメントがテキスト領域抽出をサポートしている場合、#getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) を呼び出し、空でないテキスト領域ごとに [TemplateField](../../com.groupdocs.parser.templates/templatefield) を 1 つ生成します。名前は {prefix}_{n}（デフォルトのプレフィックスは \"Field\"）です。各フィールドにはテキスト領域の矩形に基づく [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) が設定され、ページの幅は pageWidth として記録されるため、以降のテンプレートスケーリングが機能します。
3. ドキュメントがテキスト領域をサポートしていない場合、null を返します。

### OCR caveat

C# の実装は、ドキュメントが画像のみの場合にページプレビューに対して OCR を実行し、フィールドを導出します。Java の [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) はユーザー提供であるため、コネクタが構成されておりかつコネクタの recognizeTextAreas(...) が適切な矩形を返す場合にのみ、OCR 駆動の生成は意味があります。options.getOcrOptions() が設定され、コネクタが利用可能なときは、OCR パイプラインが優先されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | 生成オプションです。null の場合があります（デフォルトが適用されます）。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - 生成された [TemplateItem](../../com.groupdocs.parser.templates/templateitem) のイテラブル、またはこのドキュメント形式でサポートされていない場合は null です。

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


スプレッドシート内のすべてのワークシートに関する情報を抽出します。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - スプレッドシート内のすべてのワークシートに関する情報を含む [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) インスタンスのリストです。

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


ワークシートに関する情報を抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | worksheetIndex | int | ワークシートのゼロベースインデックスです。 |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


ワークシートのセルを抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | worksheetIndex | int | ワークシートのゼロベースインデックスです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - セルデータを含む [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) インスタンスのコレクションです。

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


カスタマイズオプションを使用して、ワークシートのセルを抽出します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | worksheetIndex | int | ワークシートのゼロベースインデックスです。 |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | ワークシート抽出オプションです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - セルデータを含む [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) インスタンスのコレクションです。

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


ユーザー生成テンプレートでドキュメントを解析します。

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | ユーザー生成テンプレートです。 |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


提供されたオプションを使用して、ユーザー生成テンプレートでドキュメントを解析します。

もし
options.getPageIndex()
が設定されている場合、そのページのみが解析されます。設定されていない場合はすべてのページが解析されます。

OCR のサポートは、[ParserSettings](../../com.groupdocs.parser.options/parsersettings) で構成された [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) に依存します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | ユーザー生成テンプレートです。 |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | パース バイ テンプレート オプションです。 |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


コレクションから最適なテンプレートを自動的に選択してドキュメントを解析します。

C# のミラー
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
コミット 71f3f21 で導入されました。

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions)、そして生成されるテンプレート
最も多くの入力済みフィールド（null でないページ領域でテキストが空でないもの）の数が多いものが勝ちます。C# の実装は使用します。
OCR パスに対する hidden-marker のマッチング；このパスは hidden-field マーカーが原因で、Java ではまだ利用できません。
OCR 主導の TemplatePageOcrParser は移植されていないため、この入力済みフィールド数が透過的なフォールバックとして使用されます。
C# と同一の動作が必要な呼び出し元は、OCR エンジンが接続されたらカスタムセレクタを組み込むべきです。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | 候補テンプレートのコレクションです。パーサーは最も適合するものを選択します。 |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | パースオプションです。null の可能性があります。 |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


ドキュメントフォームを解析します。

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

以下の例は、ドキュメントのフォームをパースする方法を示しています。

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


ドキュメントから構造化テキストを抽出します。

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - XML テキスト構造を持つ org.w3c.dom.Document クラスのインスタンスです。テキスト構造の抽出がサポートされていない場合は null です。

### close() {#close--}
```
public void close()
```


このリソースを閉じ、基になるリソースをすべて解放します。


