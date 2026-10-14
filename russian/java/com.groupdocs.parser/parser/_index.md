---
title: "Parser"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет основной класс, который управляет извлечением контейнера текстовых изображений и функциями парсинга."
type: docs
weight: 10
url: /ru/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

Представляет основной класс, который управляет функциями извлечения текста, изображений, контейнеров и их разбора.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL с  loadOptions . |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL с  parserSettings . |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL с  loadOptions  и  parserSettings . |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из базы данных. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из базы данных. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions) и [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions) и [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | Возвращает общую информацию о файле. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | Возвращает общую информацию о файле. |
|
|  | [getFeatures()](#getFeatures--) | Получает поддерживаемые функции. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | Создаёт предварительный просмотр страницы документа. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | Создаёт предварительный просмотр страницы документа с использованием параметров настройки. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | Получить предварительный просмотр страниц. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Возвращает общую информацию о документе. |
|
|  | [getText()](#getText--) | Извлекает текст из документа. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | Извлекает страницу текста из документа с использованием параметров текста (для включения режима быстрой необработанной извлечения текста). |
|
|  | [getText(int pageIndex)](#getText-int-) | Извлекает текст со страницы документа. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | Извлекает текст со страницы документа с использованием параметров текста (для включения режима быстрой необработанной извлечения текста). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | Извлекает отформатированный текст из документа. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | Извлекает отформатированный текст со страницы документа. |
|
|  | [search(String keyword)](#search-java.lang.String-) | Ищет ключевое слово в документе. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | Ищет ключевое слово в документе с использованием параметров поиска (регулярное выражение, учёт регистра и т.д.). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | Извлекает выделение из документа. |
|
|  | [getToc()](#getToc--) | Извлекает оглавление из документа. |
|
|  | [getMetadata()](#getMetadata--) | Извлекает метаданные из документа. |
|
|  | [getAnnotations()](#getAnnotations--) | Извлекает аннотации из документа. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | Извлекает аннотации со страницы документа. |
|
|  | [getContainer()](#getContainer--) | Извлекает объект‑контейнер из документа для работы с форматами, содержащими вложения, ZIP‑архивы и т.п. |
|
|  | [getTextAreas()](#getTextAreas--) | Извлекает текстовые области из документа. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | Извлекает текстовые области из документа, используя параметры настройки (регулярное выражение, учет регистра и т.д.). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | Извлекает текстовые области со страницы документа. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | Извлекает текстовые области со страницы документа, используя параметры настройки (регулярное выражение, учет регистра и т.д.). |
|
|  | [getImages()](#getImages--) | Извлекает изображения из документа. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | Извлекает изображения из документа, используя параметры настройки (для задания прямоугольной области, содержащей изображения). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | Извлекает изображения со страницы документа. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | Извлекает изображения со страницы документа, используя параметры настройки (для задания прямоугольной области, содержащей изображения). |
|
|  | [getHyperlinks()](#getHyperlinks--) | Извлекает гиперссылки из документа. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | Извлекает гиперссылки со страницы документа. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | Извлекает гиперссылки из документа, используя параметры настройки (для задания прямоугольной области, содержащей гиперссылки). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | Извлекает гиперссылки со страницы документа, используя параметры настройки (для задания прямоугольной области, содержащей гиперссылки). |
|
|  | [getBarcodes()](#getBarcodes--) | Извлекает штрихкоды из документа. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | Извлекает штрихкоды со страницы документа. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | Извлекает штрихкоды из документа, используя параметры настройки (для задания прямоугольной области, содержащей штрихкоды). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | Извлекает штрихкоды со страницы документа, используя параметры настройки (для задания прямоугольной области, содержащей штрихкоды). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | Извлекает таблицы из документа. |
|
|  | [getTables()](#getTables--) | Извлекает таблицы из документа, автоматически определяя их. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | Извлекает таблицы со страницы документа. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | Извлекает таблицы со страницы документа, автоматически определяя их. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | Создает коллекцию корректирующих [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s для документа. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | Извлекает информацию обо всех листах в таблице. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | Извлекает информацию о листе. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | Извлекает ячейки листа. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | Извлекает ячейки листа, используя параметры настройки. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | Разбирает документ с помощью шаблона, созданного пользователем. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | Разбирает документ с помощью шаблона, созданного пользователем, с указанными параметрами. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | Разбирает документ, автоматически выбирая наиболее подходящий шаблон из коллекции. |
|
|  | [parseForm()](#parseForm--) | Разбирает форму документа. |
|
|  | [getStructure()](#getStructure--) | Извлекает структурированный текст из документа. |
|
|  | [close()](#close--) | Закрывает этот ресурс, освобождая все связанные ресурсы. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | url | java.net.URL | URL, на который отправляется запрос |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL с  loadOptions .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | url | java.net.URL | URL, на который отправляется запрос. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия файла. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL с  parserSettings .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | url | java.net.URL | URL, на который отправляется запрос. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из URL с  loadOptions  и  parserSettings .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | url | java.net.URL | URL, на который отправляется запрос. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия файла. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из базы данных.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

Следующий пример показывает, как извлечь данные из базы данных Sqlite:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | соединение | java.sql.Connection | Подключение к базе данных. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) для извлечения данных из базы данных.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Следующий пример показывает, как извлечь данные из базы данных Sqlite:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | соединение | java.sql.Connection | Подключение к базе данных. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

Следующий пример показывает, как извлечь электронные письма из Exchange Server:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Подключение к электронной почте. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Следующий пример показывает, как извлечь электронные письма из Exchange Server:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | Подключение к электронной почте. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

Следующий пример показывает, как загрузить документ с локального диска:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

Пароль документа передаётся классом [LoadOptions](../../com.groupdocs.parser.options/loadoptions):

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия файла. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions) и [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Следующий пример показывает, как получить информацию через интерфейс [ILogger](../../com.groupdocs.parser.options/ilogger):

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия файла. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

Следующий пример показывает, как загрузить документ из потока:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | документ | java.io.InputStream | Исходный входной поток. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

В некоторых случаях необходимо определить [FileFormat](../../com.groupdocs.parser.options/fileformat). Также для специальных случаев (базы данных, сервер электронной почты)
и для определения типов файлов по содержимому:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | документ | java.io.InputStream | Исходный входной поток. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия файла. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | документ | java.io.InputStream | Исходный входной поток. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


Инициализирует новый экземпляр класса [Parser](../../com.groupdocs.parser/parser) с [LoadOptions](../../com.groupdocs.parser.options/loadoptions) и [ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

Следующий пример показывает, как получить информацию через интерфейс [ILogger](../../com.groupdocs.parser.options/ilogger):

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | документ | java.io.InputStream | Исходный входной поток. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия файла. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


Возвращает общую информацию о файле.

Следующий код показывает, как проверить, защищён ли файл паролем:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


Возвращает общую информацию о файле.

Следующий код показывает, как проверить, защищён ли файл паролем:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | документ | java.io.InputStream | Исходный входной поток. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


Получает поддерживаемые функции.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

Если функция не поддерживается, метод возвращает
null
вместо значения. Некоторые операции могут потреблять
значительное время. Поэтому не оптимально вызывать метод только для проверки поддержки функции.
Для этой цели используется свойство Features:

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


Создаёт предварительный просмотр страницы документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.io.OutputStream — экземпляр java.io.OutputStream, содержащий изображение страницы документа;  null  если генерация предварительного просмотра страницы не поддерживается.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


Создаёт предварительный просмотр страницы документа с использованием параметров настройки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Параметры для настройки генерации предварительного просмотра. |
|

**Returns:**
java.io.OutputStream — экземпляр java.io.OutputStream, содержащий изображение страницы документа;  null  если генерация предварительного просмотра страницы не поддерживается.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


Получить предварительный просмотр страниц.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | Параметры для установки требований и делегатов потоков при генерации предварительного просмотра. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


Возвращает общую информацию о документе.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

В следующем примере показано, как получить информацию о документе:

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


Извлекает текст из документа.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

В следующем примере показано, как извлечь текст из документа:

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


Извлекает страницу текста из документа с использованием параметров текста (для включения режима быстрой необработанной извлечения текста).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

В следующем примере показано, как извлечь необработанный текст из документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Параметры извлечения текста. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


Извлекает текст со страницы документа.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

В следующем примере показано, как извлечь текст со страницы документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


Извлекает текст со страницы документа с использованием параметров текста (для включения режима быстрой необработанной извлечения текста).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

В следующем примере показано, как извлечь необработанный текст со страницы документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | Параметры извлечения текста. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


Извлекает отформатированный текст из документа.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

В следующем примере показано, как извлечь текст документа в виде HTML:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Параметры извлечения отформатированного текста. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


Извлекает отформатированный текст со страницы документа.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

В следующем примере показано, как извлечь текст страницы документа в виде Markdown:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | Параметры извлечения отформатированного текста. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


Ищет ключевое слово в документе.

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

В следующем примере показано, как найти ключевое слово в документе:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | ключевое слово | java.lang.String | Ключевое слово для поиска. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> — коллекция объектов [SearchResult](../../com.groupdocs.parser.data/searchresult);  null  если поиск не поддерживается.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


Ищет ключевое слово в документе с использованием параметров поиска (регулярное выражение, учёт регистра и т.д.).

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

В следующем примере показано, как выполнить поиск с регулярным выражением в документе:

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

В следующем примере показано, как искать текст на страницах:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | ключевое слово | java.lang.String | Ключевое слово для поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | Параметры поиска. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> — коллекция объектов [SearchResult](../../com.groupdocs.parser.data/searchresult);  null  если поиск не поддерживается.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


Извлекает выделение из документа.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

В следующем примере показано, как извлечь выделение, содержащее 3 слова:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | позиция | int | Начальная позиция выделения. |
|
|  | isDirect | boolean | Значение, указывающее, является ли извлечение выделения прямым.  true  если выделение извлекается справа от позиции; в противном случае  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры извлечения выделения. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


Извлекает оглавление из документа.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

В следующем примере показано, как извлечь оглавление из файла EPUB:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - Коллекция элементов оглавления;  null  если извлечение оглавления не поддерживается.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Извлекает метаданные из документа.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

В следующем примере показано, как извлечь метаданные из документа:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Коллекция элементов метаданных;  null  если извлечение метаданных не поддерживается.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


Извлекает аннотации из документа.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Коллекция элементов аннотаций;  null  если извлечение аннотаций не поддерживается.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


Извлекает аннотации со страницы документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - Коллекция элементов аннотаций;  null  если извлечение аннотаций не поддерживается.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


Извлекает объект‑контейнер из документа для работы с форматами, содержащими вложения, ZIP‑архивы и т.п.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

В следующем примере показано, как извлечь текст из zip‑объектов:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - Коллекция элементов контейнера;  null  если извлечение контейнера не поддерживается.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


Извлекает текстовые области из документа.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

В следующем примере показано, как извлечь все текстовые области из всего документа:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Коллекция объектов [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  если извлечение текстовых областей не поддерживается.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


Извлекает текстовые области из документа, используя параметры настройки (регулярное выражение, учет регистра и т.д.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

В следующем примере показано, как извлечь только текстовые области с цифрами из верхнего левого угла:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Параметры извлечения текстовых областей. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Коллекция объектов [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  если извлечение текстовых областей не поддерживается.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


Извлекает текстовые области со страницы документа.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

Для извлечения текстовых областей со страницы документа используется следующий метод:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Коллекция объектов [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  если извлечение текстовых областей не поддерживается.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


Извлекает текстовые области со страницы документа, используя параметры настройки (регулярное выражение, учет регистра и т.д.).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | Параметры извлечения текстовых областей. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Коллекция объектов [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  если извлечение текстовых областей не поддерживается.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


Извлекает изображения из документа.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

В следующем примере показано, как извлечь все изображения из всего документа:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Коллекция объектов [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  если извлечение изображений не поддерживается.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


Извлекает изображения из документа, используя параметры настройки (для задания прямоугольной области, содержащей изображения).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

В следующем примере показано, как извлечь только изображения из верхнего левого угла:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Параметры извлечения изображений. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Коллекция объектов [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  если извлечение изображений не поддерживается.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


Извлекает изображения со страницы документа.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

Для извлечения изображений со страницы документа используется следующий метод:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Коллекция объектов [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  если извлечение изображений не поддерживается.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


Извлекает изображения со страницы документа, используя параметры настройки (для задания прямоугольной области, содержащей изображения).

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Параметры извлечения изображений. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - Коллекция объектов [PageImageArea](../../com.groupdocs.parser.data/pageimagearea);  null  если извлечение изображений не поддерживается.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


Извлекает гиперссылки из документа.

В следующем примере показано, как извлечь все гиперссылки из всего документа:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Коллекция объектов [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  если извлечение гиперссылок не поддерживается.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


Извлекает гиперссылки со страницы документа.

В следующем примере показано, как извлечь гиперссылки со страницы документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Коллекция объектов [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  если извлечение гиперссылок не поддерживается.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


Извлекает гиперссылки из документа, используя параметры настройки (для задания прямоугольной области, содержащей гиперссылки).

В следующем примере показано, как извлечь гиперссылки из области страницы документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Параметры извлечения гиперссылок. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Коллекция объектов [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  если извлечение гиперссылок не поддерживается.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


Извлекает гиперссылки со страницы документа, используя параметры настройки (для задания прямоугольной области, содержащей гиперссылки).

В следующем примере показано, как извлекать гиперссылки из области страницы документа, используя параметры настройки:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | Параметры извлечения гиперссылок. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - Коллекция объектов [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea);  null  если извлечение гиперссылок не поддерживается.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


Извлекает штрихкоды из документа.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Коллекция объектов [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  если извлечение штрихкодов не поддерживается.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


Извлекает штрихкоды со страницы документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Коллекция объектов [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  если извлечение штрихкодов не поддерживается.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


Извлекает штрихкоды из документа, используя параметры настройки (для задания прямоугольной области, содержащей штрихкоды).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Параметры извлечения штрихкодов. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Коллекция объектов [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  если извлечение штрихкодов не поддерживается.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


Извлекает штрихкоды со страницы документа, используя параметры настройки (для задания прямоугольной области, содержащей штрихкоды).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | Параметры извлечения штрихкодов. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - Коллекция объектов [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea);  null  если извлечение штрихкодов не поддерживается.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


Извлекает таблицы из документа.

В следующем примере показано, как извлекать таблицы из всего документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Параметры извлечения таблиц. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Коллекция объектов [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  если извлечение таблиц не поддерживается.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


Извлекает таблицы из документа, автоматически определяя их.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Коллекция объектов [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  если извлечение таблиц не поддерживается.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


Извлекает таблицы со страницы документа.

В следующем примере показано, как извлекать таблицы со страницы документа:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | Параметры извлечения таблиц. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Коллекция объектов [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  если извлечение таблиц не поддерживается.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


Извлекает таблицы со страницы документа, автоматически определяя их.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pageIndex | int | Индекс страницы, начинающийся с нуля. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - Коллекция объектов [PageTableArea](../../com.groupdocs.parser.data/pagetablearea);  null  если извлечение таблиц не поддерживается.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


Создает коллекцию корректирующих [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s для документа.

Java‑зеркало C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (коммиты d4e691b /
ae9e98c). Полезный как шаблон отправной точки, который пользователь может затем обрезать или переименовать.

### Algorithm

1. Выберите страницу из  options.getPageIndex()  (по умолчанию  0 ).
2. Если документ поддерживает извлечение текстовых областей, вызовите #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) и создайте один [TemplateField](../../com.groupdocs.parser.templates/templatefield) для каждой непустой текстовой области, названный  {prefix}_{n}  (префикс по умолчанию  "Field" ). Каждый поле получает [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) в прямоугольнике текстовой области, при этом ширина страницы фиксируется как  pageWidth  чтобы последующее масштабирование шаблона работало.
3. Если документ не поддерживает текстовые области, верните  null .

### OCR caveat

Реализация на C# выполняет OCR над предварительным просмотром страницы, чтобы получить поля, когда документ состоит только из изображений. [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) в Java предоставляется пользователем, поэтому генерация на основе OCR имеет смысл только если коннектор настроен И метод коннектора  recognizeTextAreas(...)  возвращает корректные прямоугольники. Когда  options.getOcrOptions()  установлен и коннектор доступен, предпочтителен OCR‑конвейер.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | Параметры генерации. Может быть  null  (применены значения по умолчанию). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - Итерабельный набор сгенерированных [TemplateItem](../../com.groupdocs.parser.templates/templateitem)ов, или  null  если данный формат документа не поддерживается.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


Извлекает информацию обо всех листах в таблице.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - Список экземпляров [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo), содержащих информацию обо всех листах в таблице.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


Извлекает информацию о листе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | worksheetIndex | int | Нулевой индекс листа. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


Извлекает ячейки листа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | worksheetIndex | int | Нулевой индекс листа. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Коллекция экземпляров [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell), содержащих данные ячеек.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


Извлекает ячейки листа, используя параметры настройки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | worksheetIndex | int | Нулевой индекс листа. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | Параметры извлечения листа. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - Коллекция экземпляров [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell), содержащих данные ячеек.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


Разбирает документ с помощью шаблона, созданного пользователем.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Шаблон, созданный пользователем. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


Разбирает документ с помощью шаблона, созданного пользователем, с указанными параметрами.

Если
options.getPageIndex()
установлен, только эта страница обрабатывается; в противном случае обрабатываются все страницы.

Поддержка OCR зависит от [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase), настроенного в [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | Шаблон, созданный пользователем. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Опции парсинга по шаблону. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


Разбирает документ, автоматически выбирая наиболее подходящий шаблон из коллекции.

Отображение C#.
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
введено в коммите 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), и шаблон, который дает
выигрывает шаблон с наибольшим количеством заполненных полей (не‑null областей страницы с непустым текстом). Реализация на C# использует
сопоставление скрытых маркеров с проходом OCR; этот путь пока недоступен в Java, потому что скрытые маркеры полей и
TemplatePageOcrParser, управляемый OCR, не портирован, поэтому используется этот подсчёт заполненных полей как прозрачный резерв.
Вызывающие, которым необходимо поведение, идентичное C#, должны подключить пользовательский селектор после подключения OCR‑движка.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | Коллекция кандидатных шаблонов. Парсер выберет наиболее подходящий. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | Опции парсинга. Может быть null. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


Разбирает форму документа.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

Следующий пример показывает, как разобрать форму документа:

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


Извлекает структурированный текст из документа.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document — экземпляр класса  org.w3c.dom.Document  с XML‑текстовой структурой; null, если извлечение текстовой структуры не поддерживается.

### close() {#close--}
```
public void close()
```


Закрывает этот ресурс, освобождая все связанные ресурсы.


