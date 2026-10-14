---
title: "Parser"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل الفئة الرئيسية التي تتحكم في استخراج حاوية النصوص والصور ووظيفة التحليل."
type: docs
weight: 10
url: /ar/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

يمثل الفئة الرئيسية التي تتحكم في النصوص والصور واستخراج الحاويات ووظيفة التحليل.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL مع  loadOptions . |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL مع  parserSettings . |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL مع  loadOptions  و  parserSettings . |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من قاعدة بيانات. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من قاعدة بيانات. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions) و[ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions) و[ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | يرجع المعلومات العامة حول ملف. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | يرجع المعلومات العامة حول ملف. |
|
|  | [getFeatures()](#getFeatures--) | يحصل على الميزات المدعومة. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | ينشئ معاينة لصفحة المستند. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | ينشئ معاينة لصفحة المستند باستخدام خيارات التخصيص. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | احصل على معاينة الصفحات. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | يرجع المعلومات العامة حول المستند. |
|
|  | [getText()](#getText--) | يستخرج نصًا من المستند. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | يستخرج صفحة نصية من المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع). |
|
|  | [getText(int pageIndex)](#getText-int-) | يستخرج نصًا من صفحة المستند. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | يستخرج نصًا من صفحة المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | يستخرج نصًا منسقًا من المستند. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | يستخرج نصًا منسقًا من صفحة المستند. |
|
|  | [search(String keyword)](#search-java.lang.String-) | يبحث عن كلمة مفتاحية في المستند. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | يبحث عن كلمة مفتاحية في المستند باستخدام خيارات البحث (تعبير عادي، مطابقة الحالة، إلخ). |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | يستخرج تمييزًا من المستند. |
|
|  | [getToc()](#getToc--) | يستخرج جدول محتويات من المستند. |
|
|  | [getMetadata()](#getMetadata--) | يستخرج بيانات التعريف من المستند. |
|
|  | [getAnnotations()](#getAnnotations--) | يستخرج التعليقات التوضيحية من المستند. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | يستخرج التعليقات التوضيحية من صفحة المستند. |
|
|  | [getContainer()](#getContainer--) | يستخرج كائن حاوية من المستند للعمل مع الصيغ التي تحتوي على مرفقات، أرشيفات ZIP، إلخ. |
|
|  | [getTextAreas()](#getTextAreas--) | يستخرج مناطق النص من المستند. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | يستخرج مناطق النص من المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ). |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | يستخرج مناطق النص من صفحة المستند. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | يستخرج مناطق النص من صفحة المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ). |
|
|  | [getImages()](#getImages--) | يستخرج الصور من المستند. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | يستخرج الصور من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور). |
|
|  | [getImages(int pageIndex)](#getImages-int-) | يستخرج الصور من صفحة المستند. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | يستخرج الصور من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور). |
|
|  | [getHyperlinks()](#getHyperlinks--) | يستخرج الروابط التشعبية من المستند. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | يستخرج الروابط التشعبية من صفحة المستند. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | يستخرج الروابط التشعبية من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية). |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | يستخرج الروابط التشعبية من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية). |
|
|  | [getBarcodes()](#getBarcodes--) | يستخرج الرموز الشريطية من المستند. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | يستخرج الرموز الشريطية من صفحة المستند. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | يستخرج الرموز الشريطية من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الرموز الشريطية). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | يستخرج الرموز الشريطية من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الرموز الشريطية). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | يستخرج الجداول من المستند. |
|
|  | [getTables()](#getTables--) | يستخرج الجداول من المستند، مع اكتشافها تلقائيًا. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | يستخرج الجداول من صفحة المستند. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | يستخرج الجداول من صفحة المستند، مع اكتشافها تلقائيًا. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | ينشئ مجموعة من التعديلات [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s للمستند. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | يستخرج المعلومات حول جميع أوراق العمل في جدول البيانات. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | يستخرج المعلومات حول ورقة العمل. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | يستخرج خلايا ورقة العمل. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | يستخرج خلايا ورقة العمل باستخدام خيارات التخصيص. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | يقوم بتحليل المستند باستخدام القالب الذي أنشأه المستخدم. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | يقوم بتحليل المستند باستخدام القالب الذي أنشأه المستخدم مع الخيارات المقدمة. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | يقوم بتحليل المستند عن طريق اختيار القالب الأنسب تلقائيًا من مجموعة. |
|
|  | [parseForm()](#parseForm--) | يقوم بتحليل نموذج المستند. |
|
|  | [getStructure()](#getStructure--) | يستخرج نصًا منظمًا من المستند. |
|
|  | [close()](#close--) | يغلق هذا المورد، متخليًا عن أي موارد أساسية. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | url | java.net.URL | عنوان URL الذي يُرسل إليه الطلب |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL مع  loadOptions .


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | url | java.net.URL | عنوان URL الذي يُرسل إليه الطلب. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح الملف. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL مع  parserSettings .


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | url | java.net.URL | عنوان URL الذي يُرسل إليه الطلب. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


يُنشئ مثيلًا جديدًا من الفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من عنوان URL مع  loadOptions  و  parserSettings .


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | url | java.net.URL | عنوان URL الذي يُرسل إليه الطلب. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح الملف. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من قاعدة بيانات.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

المثال التالي يوضح كيفية استخراج البيانات من قاعدة بيانات Sqlite:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الاتصال | java.sql.Connection | اتصال قاعدة البيانات. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) لاستخراج البيانات من قاعدة بيانات.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

المثال التالي يوضح كيفية استخراج البيانات من قاعدة بيانات Sqlite:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الاتصال | java.sql.Connection | اتصال قاعدة البيانات. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

المثال التالي يوضح كيفية استخراج رسائل البريد الإلكتروني من خادم Exchange:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | اتصال البريد الإلكتروني. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

المثال التالي يوضح كيفية استخراج رسائل البريد الإلكتروني من خادم Exchange:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | اتصال البريد الإلكتروني. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

المثال التالي يوضح كيفية تحميل المستند من القرص المحلي:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

كلمة مرور المستند يتم تمريرها عبر الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions):

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح الملف. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions) و[ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

المثال التالي يوضح كيفية استلام المعلومات عبر الواجهة [ILogger](../../com.groupdocs.parser.options/ilogger):

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح الملف. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

المثال التالي يوضح كيفية تحميل المستند من الدفق:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

في بعض الحالات من الضروري تعريف [FileFormat](../../com.groupdocs.parser.options/fileformat). لكل من الحالات الخاصة (قواعد البيانات، خادم البريد الإلكتروني)
وللكشف عن أنواع الملفات بناءً على المحتوى:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح الملف. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


يُنشئ مثيلاً جديدًا لفئة [Parser](../../com.groupdocs.parser/parser) باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions) و[ParserSettings](../../com.groupdocs.parser.options/parsersettings).

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

المثال التالي يوضح كيفية استلام المعلومات عبر الواجهة [ILogger](../../com.groupdocs.parser.options/ilogger):

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح الملف. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


يرجع المعلومات العامة حول ملف.

الكود التالي يوضح كيفية التحقق مما إذا كان الملف محميًا بكلمة مرور:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


يرجع المعلومات العامة حول ملف.

الكود التالي يوضح كيفية التحقق مما إذا كان الملف محميًا بكلمة مرور:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | المستند | java.io.InputStream | دفق الإدخال المصدر. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


يحصل على الميزات المدعومة.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

إذا لم يكن الدعم للميزة متاحًا، تُعيد الطريقة
null
بدلاً من القيمة. قد تستهلك بعض العمليات
وقتًا كبيرًا. لذا ليس من المثالي استدعاء الطريقة فقط للتحقق من دعم الميزة.
لهذا الغرض تُستخدم الخاصية Features:

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


ينشئ معاينة لصفحة المستند.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.io.OutputStream - مثال من java.io.OutputStream يحتوي على صورة لصفحة المستند؛  null  إذا لم يكن توليد معاينة الصفحة مدعومًا.

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


ينشئ معاينة لصفحة المستند باستخدام خيارات التخصيص.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | الخيارات لتخصيص توليد المعاينة. |
|

**Returns:**
java.io.OutputStream - مثال من java.io.OutputStream يحتوي على صورة لصفحة المستند؛  null  إذا لم يكن توليد معاينة الصفحة مدعومًا.

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


احصل على معاينة الصفحات.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | الخيارات لتعيين المتطلبات ومندوبات الدفق لتوليد المعاينة. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


يرجع المعلومات العامة حول المستند.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

المثال التالي يوضح كيفية الحصول على معلومات المستند:

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


يستخرج نصًا من المستند.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

المثال التالي يوضح كيفية استخراج نص من مستند:

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


يستخرج صفحة نصية من المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

المثال التالي يوضح كيفية استخراج نص خام من مستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | خيارات استخراج النص. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


يستخرج نصًا من صفحة المستند.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

المثال التالي يوضح كيفية استخراج نص من صفحة المستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


يستخرج نصًا من صفحة المستند باستخدام خيارات النص (لتمكين وضع استخراج النص الخام السريع).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

المثال التالي يوضح كيفية استخراج نص خام من صفحة المستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | خيارات استخراج النص. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


يستخرج نصًا منسقًا من المستند.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

المثال التالي يوضح كيفية استخراج نص المستند كنص HTML:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | خيارات استخراج النص المنسق. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


يستخرج نصًا منسقًا من صفحة المستند.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

المثال التالي يوضح كيفية استخراج نص صفحة المستند كنص Markdown:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | خيارات استخراج النص المنسق. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


يبحث عن كلمة مفتاحية في المستند.

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

المثال التالي يوضح كيفية العثور على كلمة مفتاحية في مستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | كلمة مفتاحية | java.lang.String | الكلمة المفتاحية للبحث. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - مجموعة من كائنات [SearchResult](../../com.groupdocs.parser.data/searchresult)؛  null  إذا لم يكن البحث مدعومًا.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


يبحث عن كلمة مفتاحية في المستند باستخدام خيارات البحث (تعبير عادي، مطابقة الحالة، إلخ).

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

المثال التالي يوضح كيفية البحث باستخدام تعبير عادي في مستند:

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

المثال التالي يوضح كيفية البحث عن نص في الصفحات:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | كلمة مفتاحية | java.lang.String | الكلمة المفتاحية للبحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | خيارات البحث. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - مجموعة من كائنات [SearchResult](../../com.groupdocs.parser.data/searchresult)؛  null  إذا لم يكن البحث مدعومًا.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


يستخرج تمييزًا من المستند.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

المثال التالي يوضح كيفية استخراج تمييز يحتوي على 3 كلمات:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | int | موضع البداية للتمييز. |
|
|  | isDirect | boolean | القيمة التي تشير إلى ما إذا كان استخراج الـ higlight مباشرًا.  true  إذا تم استخراج الـ higlight من اليمين من الموضع؛ وإلا،  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | خيارات استخراج التمييز. |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


يستخرج جدول محتويات من المستند.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

المثال التالي يوضح كيفية استخراج جدول المحتويات من ملف EPUB:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - مجموعة من عناصر جدول المحتويات؛  null  إذا لم يكن استخراج جدول المحتويات مدعومًا.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


يستخرج بيانات التعريف من المستند.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

المثال التالي يوضح كيفية استخراج البيانات الوصفية من مستند:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - مجموعة من عناصر البيانات الوصفية؛  null  إذا لم يكن استخراج البيانات الوصفية مدعومًا.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


يستخرج التعليقات التوضيحية من المستند.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - مجموعة من عناصر التعليقات التوضيحية؛  null  إذا لم يكن استخراج التعليقات التوضيحية مدعومًا.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


يستخرج التعليقات التوضيحية من صفحة المستند.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - مجموعة من عناصر التعليقات التوضيحية؛  null  إذا لم يكن استخراج التعليقات التوضيحية مدعومًا.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


يستخرج كائن حاوية من المستند للعمل مع الصيغ التي تحتوي على مرفقات، أرشيفات ZIP، إلخ.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

المثال التالي يوضح كيفية استخراج نص من كيانات zip:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - مجموعة من عناصر الحاوية؛  null  إذا لم يكن استخراج الحاوية مدعومًا.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


يستخرج مناطق النص من المستند.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

المثال التالي يوضح كيفية استخراج جميع مناطق النص من المستند بالكامل:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - مجموعة من كائنات [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)؛  null  إذا لم يكن استخراج مناطق النص مدعومًا.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


يستخرج مناطق النص من المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

المثال التالي يوضح كيفية استخراج مناطق النص التي تحتوي على أرقام فقط من الزاوية العليا اليسرى:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | خيارات استخراج مناطق النص. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - مجموعة من كائنات [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)؛  null  إذا لم يكن استخراج مناطق النص مدعومًا.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


يستخرج مناطق النص من صفحة المستند.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

لاستخراج مناطق النص من صفحة المستند يتم استخدام الطريقة التالية:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - مجموعة من كائنات [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)؛  null  إذا لم يكن استخراج مناطق النص مدعومًا.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


يستخرج مناطق النص من صفحة المستند باستخدام خيارات التخصيص (التعبير النمطي، مطابقة الحالة، إلخ).

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | خيارات استخراج مناطق النص. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - مجموعة من كائنات [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)؛  null  إذا لم يكن استخراج مناطق النص مدعومًا.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


يستخرج الصور من المستند.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

المثال التالي يوضح كيفية استخراج جميع الصور من المستند بالكامل:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - مجموعة من كائنات [PageImageArea](../../com.groupdocs.parser.data/pageimagearea)؛  null  إذا لم يكن استخراج الصور مدعومًا.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


يستخرج الصور من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور).

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

المثال التالي يوضح كيفية استخراج الصور فقط من الزاوية العليا اليسرى:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | خيارات استخراج الصور. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - مجموعة من كائنات [PageImageArea](../../com.groupdocs.parser.data/pageimagearea)؛  null  إذا لم يكن استخراج الصور مدعومًا.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


يستخرج الصور من صفحة المستند.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

لاستخراج الصور من صفحة المستند يتم استخدام الطريقة التالية:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - مجموعة من كائنات [PageImageArea](../../com.groupdocs.parser.data/pageimagearea)؛  null  إذا لم يكن استخراج الصور مدعومًا.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


يستخرج الصور من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الصور).

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | خيارات استخراج الصور. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - مجموعة من كائنات [PageImageArea](../../com.groupdocs.parser.data/pageimagearea)؛  null  إذا لم يكن استخراج الصور مدعومًا.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


يستخرج الروابط التشعبية من المستند.

المثال التالي يوضح كيفية استخراج جميع الروابط التشعبية من المستند بالكامل:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - مجموعة من كائنات [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea)؛  null  إذا لم يكن استخراج الروابط التشعبية مدعومًا.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


يستخرج الروابط التشعبية من صفحة المستند.

المثال التالي يوضح كيفية استخراج الروابط التشعبية من صفحة المستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - مجموعة من كائنات [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea)؛  null  إذا لم يكن استخراج الروابط التشعبية مدعومًا.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


يستخرج الروابط التشعبية من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية).

المثال التالي يوضح كيفية استخراج الروابط التشعبية من منطقة صفحة المستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | خيارات استخراج الروابط التشعبية. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - مجموعة من كائنات [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea)؛  null  إذا لم يكن استخراج الروابط التشعبية مدعومًا.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


يستخرج الروابط التشعبية من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الروابط التشعبية).

المثال التالي يوضح كيفية استخراج الروابط التشعبية من مساحة صفحة المستند باستخدام خيارات التخصيص:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | خيارات استخراج الروابط التشعبية. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - مجموعة من كائنات [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea)؛  null  إذا لم يكن استخراج الروابط التشعبية مدعومًا.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


يستخرج الرموز الشريطية من المستند.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - مجموعة من كائنات [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea)؛  null  إذا لم يكن استخراج الباركود مدعومًا.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


يستخرج الرموز الشريطية من صفحة المستند.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - مجموعة من كائنات [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea)؛  null  إذا لم يكن استخراج الباركود مدعومًا.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


يستخرج الرموز الشريطية من المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الرموز الشريطية).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | الخيارات الخاصة باستخراج الباركود. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - مجموعة من كائنات [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea)؛  null  إذا لم يكن استخراج الباركود مدعومًا.\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


يستخرج الرموز الشريطية من صفحة المستند باستخدام خيارات التخصيص (لتحديد المنطقة المستطيلة التي تحتوي على الرموز الشريطية).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | الخيارات الخاصة باستخراج الباركود. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - مجموعة من كائنات [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea)؛  null  إذا لم يكن استخراج الباركود مدعومًا.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


يستخرج الجداول من المستند.

المثال التالي يوضح كيفية استخراج الجداول من المستند بالكامل:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | الخيارات الخاصة باستخراج الجداول. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - مجموعة من كائنات [PageTableArea](../../com.groupdocs.parser.data/pagetablearea)؛  null  إذا لم يكن استخراج الجداول مدعومًا.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


يستخرج الجداول من المستند، مع اكتشافها تلقائيًا.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - مجموعة من كائنات [PageTableArea](../../com.groupdocs.parser.data/pagetablearea)؛  null  إذا لم يكن استخراج الجداول مدعومًا.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


يستخرج الجداول من صفحة المستند.

المثال التالي يوضح كيفية استخراج الجداول من صفحة المستند:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | الخيارات الخاصة باستخراج الجداول. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - مجموعة من كائنات [PageTableArea](../../com.groupdocs.parser.data/pagetablearea)؛  null  إذا لم يكن استخراج الجداول مدعومًا.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


يستخرج الجداول من صفحة المستند، مع اكتشافها تلقائيًا.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - مجموعة من كائنات [PageTableArea](../../com.groupdocs.parser.data/pagetablearea)؛  null  إذا لم يكن استخراج الجداول مدعومًا.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


ينشئ مجموعة من التعديلات [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s للمستند.

نسخة Java من C#
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (التزامن d4e691b /
ae9e98c). مفيدة كقالب بداية يمكن للمستخدم بعد ذلك قصه أو إعادة تسميته.

### Algorithm

1. اختر الصفحة من  options.getPageIndex()  (الافتراضي  0 ).
2. إذا كان المستند يدعم استخراج مناطق النص، استدعِ #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) وأصدر حقلًا واحدًا من نوع [TemplateField](../../com.groupdocs.parser.templates/templatefield) لكل منطقة نص غير فارغة، باسم  {prefix}_{n}  (البادئة الافتراضية \"Field\" ). يحصل كل حقل على [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) في مستطيل منطقة النص، مع تسجيل عرض الصفحة كـ  pageWidth  حتى يعمل تحجيم القالب اللاحق بشكل صحيح.
3. إذا لم يدعم المستند مناطق النص، أعد  null .

### OCR caveat

تنفيذ C# يقوم بتشغيل OCR على معاينة الصفحة لاشتقاق الحقول عندما يكون المستند صورة فقط. الـ [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) في Java يُزود من قبل المستخدم، لذا فإن الجيل المدفوع بـ OCR يكون ذا معنى فقط إذا تم تكوين موصل وتم تكوينه بحيث تُعيد  recognizeTextAreas(...)  مستطيلات صحيحة. عندما يتم تعيين  options.getOcrOptions()  ويتوفر موصل، يُفضَّل خط أنابيب OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | خيارات التوليد. قد تكون  null  (تم تطبيق الإعدادات الافتراضية). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - مجموعة قابلة للتكرار من [TemplateItem](../../com.groupdocs.parser.templates/templateitem) المولدة، أو  null  إذا لم يكن مدعومًا من قبل تنسيق هذا المستند.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


يستخرج المعلومات حول جميع أوراق العمل في جدول البيانات.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - قائمة من كائنات [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) التي تحتوي على معلومات حول جميع أوراق العمل في جدول البيانات.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


يستخرج المعلومات حول ورقة العمل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | worksheetIndex | int | الفهرس الصفري للورقة. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


يستخرج خلايا ورقة العمل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | worksheetIndex | int | الفهرس الصفري للورقة. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - مجموعة من كائنات [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) التي تحتوي على بيانات الخلية.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


يستخرج خلايا ورقة العمل باستخدام خيارات التخصيص.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | worksheetIndex | int | الفهرس الصفري للورقة. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | خيارات استخراج الورقة. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - مجموعة من كائنات [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) التي تحتوي على بيانات الخلية.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


يقوم بتحليل المستند باستخدام القالب الذي أنشأه المستخدم.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | القالب الذي أنشأه المستخدم. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


يقوم بتحليل المستند باستخدام القالب الذي أنشأه المستخدم مع الخيارات المقدمة.

If
options.getPageIndex()
تم الضبط، يتم تحليل تلك الصفحة فقط؛ وإلا يتم تحليل جميع الصفحات.

يعتمد دعم OCR على [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) المُكوَّن في [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | القالب الذي أنشأه المستخدم. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | خيارات التحليل حسب القالب. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


يقوم بتحليل المستند عن طريق اختيار القالب الأنسب تلقائيًا من مجموعة.

نسخة متماثلة من C#
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
تم تقديمه في الالتزام 71f3f21.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions)، والقالب الذي ينتج
يفوز بأعلى عدد من الحقول المملوءة (مساحات صفحات غير فارغة مع نص غير فارغ). يستخدم تنفيذ C#
مطابقة العلامة المخفية ضد تمريرة OCR؛ هذا المسار غير متاح بعد في Java لأن علامات الحقول المخفية و
لم يتم نقل TemplatePageOcrParser المدفوع بـ OCR، لذا يُستخدم عدد الحقول المملوءة كحل احتياطي شفاف.
يجب على المستدعين الذين يحتاجون إلى سلوك مطابق لـ C# توصيل محدد مخصص بمجرد ربط محرك OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | مجموعة من القوالب المرشحة. سيختار المحلل الأنسب منها. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | خيارات التحليل. قد تكون null. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


يقوم بتحليل نموذج المستند.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

المثال التالي يوضح كيفية تحليل نموذج من المستند:

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


يستخرج نصًا منظمًا من المستند.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - مثال من فئة org.w3c.dom.Document مع بنية نص XML؛ null إذا لم يكن استخراج بنية النص مدعومًا.

### close() {#close--}
```
public void close()
```


يغلق هذا المورد، متخليًا عن أي موارد أساسية.


