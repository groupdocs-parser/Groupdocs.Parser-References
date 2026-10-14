---
title: "Parser"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트 이미지 컨테이너 추출 및 파싱 기능을 제어하는 주요 클래스를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

텍스트, 이미지, 컨테이너 추출 및 파싱 기능을 제어하는 주요 클래스를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | loadOptions와 함께 URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | parserSettings와 함께 URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | loadOptions와 parserSettings를 함께 URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | 데이터베이스에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | 데이터베이스에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | [ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions)와 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | [ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions)와 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | 파일에 대한 일반 정보를 반환합니다. |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | 파일에 대한 일반 정보를 반환합니다. |
|
|  | [getFeatures()](#getFeatures--) | 지원되는 기능을 가져옵니다. |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | 문서 페이지 미리보기를 생성합니다. |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | 맞춤 옵션을 사용하여 문서 페이지 미리보기를 생성합니다. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | 페이지 미리보기를 가져옵니다. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | 문서에 대한 일반 정보를 반환합니다. |
|
|  | [getText()](#getText--) | 문서에서 텍스트를 추출합니다. |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | 텍스트 옵션을 사용하여 문서에서 텍스트 페이지를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해). |
|
|  | [getText(int pageIndex)](#getText-int-) | 문서 페이지에서 텍스트를 추출합니다. |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | 텍스트 옵션을 사용하여 문서 페이지에서 텍스트를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해). |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | 문서에서 서식이 지정된 텍스트를 추출합니다. |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | 문서 페이지에서 서식이 지정된 텍스트를 추출합니다. |
|
|  | [search(String keyword)](#search-java.lang.String-) | 문서에서 키워드를 검색합니다. |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | 검색 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 키워드를 검색합니다. |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | 문서에서 하이라이트를 추출합니다. |
|
|  | [getToc()](#getToc--) | 문서에서 목차를 추출합니다. |
|
|  | [getMetadata()](#getMetadata--) | 문서에서 메타데이터를 추출합니다. |
|
|  | [getAnnotations()](#getAnnotations--) | 문서에서 주석을 추출합니다. |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | 문서 페이지에서 주석을 추출합니다. |
|
|  | [getContainer()](#getContainer--) | 첨부 파일, ZIP 아카이브 등을 포함하는 형식과 작업하기 위해 문서에서 컨테이너 객체를 추출합니다. |
|
|  | [getTextAreas()](#getTextAreas--) | 문서에서 텍스트 영역을 추출합니다. |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | 맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 텍스트 영역을 추출합니다. |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | 문서 페이지에서 텍스트 영역을 추출합니다. |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | 맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서 페이지에서 텍스트 영역을 추출합니다. |
|
|  | [getImages()](#getImages--) | 문서에서 이미지를 추출합니다. |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | 맞춤 옵션(이미지가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서에서 이미지를 추출합니다. |
|
|  | [getImages(int pageIndex)](#getImages-int-) | 문서 페이지에서 이미지를 추출합니다. |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | 맞춤 옵션(이미지가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서 페이지에서 이미지를 추출합니다. |
|
|  | [getHyperlinks()](#getHyperlinks--) | 문서에서 하이퍼링크를 추출합니다. |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | 문서 페이지에서 하이퍼링크를 추출합니다. |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | 맞춤 옵션(하이퍼링크가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서에서 하이퍼링크를 추출합니다. |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | 맞춤 옵션(하이퍼링크가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서 페이지에서 하이퍼링크를 추출합니다. |
|
|  | [getBarcodes()](#getBarcodes--) | 문서에서 바코드를 추출합니다. |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | 문서 페이지에서 바코드를 추출합니다. |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | 문서에서 바코드를 추출합니다(바코드가 포함된 사각형 영역을 설정하기 위한 사용자 지정 옵션 사용). |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | 문서 페이지에서 바코드를 추출합니다(바코드가 포함된 사각형 영역을 설정하기 위한 사용자 지정 옵션 사용). |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | 문서에서 표를 추출합니다. |
|
|  | [getTables()](#getTables--) | 문서에서 표를 자동으로 감지하여 추출합니다. |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | 문서 페이지에서 표를 추출합니다. |
|
|  | [getTables(int pageIndex)](#getTables-int-) | 문서 페이지에서 표를 자동으로 감지하여 추출합니다. |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | 문서를 위한 조정 [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s를 생성합니다. |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | 스프레드시트의 모든 워크시트에 대한 정보를 추출합니다. |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | 워크시트에 대한 정보를 추출합니다. |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | 워크시트 셀을 추출합니다. |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | 사용자 지정 옵션을 사용하여 워크시트 셀을 추출합니다. |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | 사용자 생성 템플릿으로 문서를 구문 분석합니다. |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | 제공된 옵션과 함께 사용자 생성 템플릿으로 문서를 구문 분석합니다. |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | 컬렉션에서 가장 일치하는 템플릿을 자동으로 선택하여 문서를 구문 분석합니다. |
|
|  | [parseForm()](#parseForm--) | 문서 양식을 구문 분석합니다. |
|
|  | [getStructure()](#getStructure--) | 문서에서 구조화된 텍스트를 추출합니다. |
|
|  | [close()](#close--) | 이 리소스를 닫고, 모든 기본 리소스를 해제합니다. |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | url | java.net.URL | 요청이 전송되는 URL |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


loadOptions와 함께 URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | url | java.net.URL | 요청이 전송되는 URL. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 파일을 열기 위한 옵션. |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


parserSettings와 함께 URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | url | java.net.URL | 요청이 전송되는 URL. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


loadOptions와 parserSettings를 함께 URL에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | url | java.net.URL | 요청이 전송되는 URL. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 파일을 열기 위한 옵션. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


데이터베이스에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

다음 예제는 Sqlite 데이터베이스에서 데이터를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 연결 | java.sql.Connection | 데이터베이스 연결입니다. |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


데이터베이스에서 데이터를 추출하기 위해 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

다음 예제는 Sqlite 데이터베이스에서 데이터를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 연결 | java.sql.Connection | 데이터베이스 연결입니다. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

다음 예제는 Exchange Server에서 이메일을 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | 이메일 연결입니다. |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

다음 예제는 Exchange Server에서 이메일을 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | 이메일 연결입니다. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

다음 예제는 로컬 디스크에서 문서를 로드하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

문서 비밀번호는 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스를 통해 전달됩니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 파일을 열기 위한 옵션. |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


[ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions)와 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

다음 예제는 [ILogger](../../com.groupdocs.parser.options/ilogger) 인터페이스를 통해 정보를 받는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 파일을 열기 위한 옵션. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

다음 예제는 스트림에서 문서를 로드하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 문서 | java.io.InputStream | 소스 입력 스트림입니다. |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

일부 경우에는 [FileFormat](../../com.groupdocs.parser.options/fileformat)을 정의해야 합니다. 데이터베이스, 이메일 서버와 같은 특수한 경우 모두
그리고 콘텐츠를 기반으로 파일 유형을 감지하기 위해:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 문서 | java.io.InputStream | 소스 입력 스트림입니다. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 파일을 열기 위한 옵션. |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


[ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 문서 | java.io.InputStream | 소스 입력 스트림입니다. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions)와 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)를 사용하여 새로운 [Parser](../../com.groupdocs.parser/parser) 클래스의 인스턴스를 초기화합니다.

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

다음 예제는 [ILogger](../../com.groupdocs.parser.options/ilogger) 인터페이스를 통해 정보를 받는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 문서 | java.io.InputStream | 소스 입력 스트림입니다. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | 파일을 열기 위한 옵션. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | 데이터 추출을 맞춤화하는 데 사용되는 파서 설정입니다. |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


파일에 대한 일반 정보를 반환합니다.

다음 코드는 파일이 비밀번호로 보호되는지 확인하는 방법을 보여줍니다:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


파일에 대한 일반 정보를 반환합니다.

다음 코드는 파일이 비밀번호로 보호되는지 확인하는 방법을 보여줍니다:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 문서 | java.io.InputStream | 소스 입력 스트림입니다. |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


지원되는 기능을 가져옵니다.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

기능이 지원되지 않으면, 메서드는 반환합니다
null
값 대신에 반환합니다. 일부 작업은 소모할 수 있습니다
많은 시간을 소요합니다. 따라서 기능 지원 여부만 확인하기 위해 메서드를 호출하는 것은 최적이 아닙니다.
이를 위해 Features 속성이 사용됩니다:

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


문서 페이지 미리보기를 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.io.OutputStream - 문서 페이지 이미지가 포함된 java.io.OutputStream 인스턴스; 페이지 미리보기 생성이 지원되지 않으면 null

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


맞춤 옵션을 사용하여 문서 페이지 미리보기를 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | 미리보기 생성을 사용자 정의하기 위한 옵션입니다. |
|

**Returns:**
java.io.OutputStream - 문서 페이지 이미지가 포함된 java.io.OutputStream 인스턴스; 페이지 미리보기 생성이 지원되지 않으면 null

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


페이지 미리보기를 가져옵니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | 미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션입니다. |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


문서에 대한 일반 정보를 반환합니다.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

다음 예제는 문서 정보를 가져오는 방법을 보여줍니다:

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


문서에서 텍스트를 추출합니다.

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

다음 예제는 문서에서 텍스트를 추출하는 방법을 보여줍니다:

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


텍스트 옵션을 사용하여 문서에서 텍스트 페이지를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

다음 예제는 문서에서 원시 텍스트를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | 텍스트 추출 옵션입니다. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


문서 페이지에서 텍스트를 추출합니다.

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

다음 예제는 문서 페이지에서 텍스트를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


텍스트 옵션을 사용하여 문서 페이지에서 텍스트를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해).

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

다음 예제는 문서 페이지에서 원시 텍스트를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | 텍스트 추출 옵션입니다. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


문서에서 서식이 지정된 텍스트를 추출합니다.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

다음 예제는 문서 텍스트를 HTML 텍스트로 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | 서식이 지정된 텍스트 추출 옵션입니다. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


문서 페이지에서 서식이 지정된 텍스트를 추출합니다.

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

다음 예제는 문서 페이지 텍스트를 Markdown 텍스트로 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | 서식이 지정된 텍스트 추출 옵션입니다. |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


문서에서 키워드를 검색합니다.

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

다음 예제는 문서에서 키워드를 찾는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 키워드 | java.lang.String | 검색할 키워드입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) 객체의 컬렉션; 검색이 지원되지 않을 경우 null.

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


검색 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 키워드를 검색합니다.

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

다음 예제는 문서에서 정규식을 사용하여 검색하는 방법을 보여줍니다:

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

다음 예제는 페이지에서 텍스트를 검색하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 키워드 | java.lang.String | 검색할 키워드입니다. |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | 검색 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) 객체의 컬렉션; 검색이 지원되지 않을 경우 null.

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


문서에서 하이라이트를 추출합니다.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

다음 예제는 3개의 단어를 포함하는 하이라이트를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 위치 | int | 하이라이트의 시작 위치입니다. |
|
|  | isDirect | boolean | 하이라이트 추출이 직접적인지 여부를 나타내는 값입니다. 위치 오른쪽에서 하이라이트가 추출되면 true, 그렇지 않으면 false. |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 하이라이트 추출 옵션입니다: |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


문서에서 목차를 추출합니다.

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

다음 예제는 EPUB 파일에서 목차를 추출하는 방법을 보여줍니다:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - 목차 항목의 컬렉션; 목차 추출이 지원되지 않을 경우 null.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


문서에서 메타데이터를 추출합니다.

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

다음 예제는 문서에서 메타데이터를 추출하는 방법을 보여줍니다:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - 메타데이터 항목의 컬렉션; 메타데이터 추출이 지원되지 않을 경우 null.

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


문서에서 주석을 추출합니다.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - 주석 항목의 컬렉션; 주석 추출이 지원되지 않을 경우 null.

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


문서 페이지에서 주석을 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - 주석 항목의 컬렉션; 주석 추출이 지원되지 않을 경우 null.

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


첨부 파일, ZIP 아카이브 등을 포함하는 형식과 작업하기 위해 문서에서 컨테이너 객체를 추출합니다.

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

다음 예제는 zip 엔터티에서 텍스트를 추출하는 방법을 보여줍니다:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - 컨테이너 항목의 컬렉션; 컨테이너 추출이 지원되지 않을 경우 null.

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


문서에서 텍스트 영역을 추출합니다.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

다음 예제는 전체 문서에서 모든 텍스트 영역을 추출하는 방법을 보여줍니다:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 객체의 컬렉션; 텍스트 영역 추출이 지원되지 않을 경우 null.

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 텍스트 영역을 추출합니다.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

다음 예제는 왼쪽 위 코너에서 숫자가 포함된 텍스트 영역만 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | 텍스트 영역 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 객체의 컬렉션; 텍스트 영역 추출이 지원되지 않을 경우 null.

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


문서 페이지에서 텍스트 영역을 추출합니다.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

문서 페이지에서 텍스트 영역을 추출하려면 다음 메서드를 사용합니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 객체의 컬렉션; 텍스트 영역 추출이 지원되지 않을 경우 null.

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서 페이지에서 텍스트 영역을 추출합니다.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | 텍스트 영역 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 객체의 컬렉션; 텍스트 영역 추출이 지원되지 않을 경우 null.

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


문서에서 이미지를 추출합니다.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

다음 예제는 전체 문서에서 모든 이미지를 추출하는 방법을 보여줍니다:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 이미지 추출이 지원되지 않을 경우 null이며, [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 객체의 컬렉션입니다.

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


맞춤 옵션(이미지가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서에서 이미지를 추출합니다.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

다음 예제는 왼쪽 위 코너에서 이미지만 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 이미지 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 이미지 추출이 지원되지 않을 경우 null이며, [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 객체의 컬렉션입니다.

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


문서 페이지에서 이미지를 추출합니다.

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

문서 페이지에서 이미지를 추출하려면 다음 메서드를 사용합니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 이미지 추출이 지원되지 않을 경우 null이며, [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 객체의 컬렉션입니다.

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


맞춤 옵션(이미지가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서 페이지에서 이미지를 추출합니다.

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 이미지 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - 이미지 추출이 지원되지 않을 경우 null이며, [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 객체의 컬렉션입니다.

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


문서에서 하이퍼링크를 추출합니다.

다음 예제는 전체 문서에서 모든 하이퍼링크를 추출하는 방법을 보여줍니다:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 하이퍼링크 추출이 지원되지 않을 경우 null이며, [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션입니다.

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


문서 페이지에서 하이퍼링크를 추출합니다.

다음 예제는 문서 페이지에서 하이퍼링크를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 하이퍼링크 추출이 지원되지 않을 경우 null이며, [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션입니다.

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


맞춤 옵션(하이퍼링크가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서에서 하이퍼링크를 추출합니다.

다음 예제는 문서 페이지 영역에서 하이퍼링크를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 하이퍼링크 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 하이퍼링크 추출이 지원되지 않을 경우 null이며, [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션입니다.

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


맞춤 옵션(하이퍼링크가 포함된 사각형 영역을 설정하기 위해)을 사용하여 문서 페이지에서 하이퍼링크를 추출합니다.

다음 예제는 사용자 지정 옵션을 사용하여 문서 페이지 영역에서 하이퍼링크를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | 하이퍼링크 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - 하이퍼링크 추출이 지원되지 않을 경우 null이며, [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션입니다.

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


문서에서 바코드를 추출합니다.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 바코드 추출이 지원되지 않을 경우 null이며, [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 객체의 컬렉션입니다.

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


문서 페이지에서 바코드를 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 바코드 추출이 지원되지 않을 경우 null이며, [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 객체의 컬렉션입니다.

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


문서에서 바코드를 추출합니다(바코드가 포함된 사각형 영역을 설정하기 위한 사용자 지정 옵션 사용).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | 바코드 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 바코드 추출이 지원되지 않을 경우 null이며, [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 객체의 컬렉션입니다.\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


문서 페이지에서 바코드를 추출합니다(바코드가 포함된 사각형 영역을 설정하기 위한 사용자 지정 옵션 사용).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | 바코드 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - 바코드 추출이 지원되지 않을 경우 null이며, [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 객체의 컬렉션입니다.

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


문서에서 표를 추출합니다.

다음 예제는 전체 문서에서 표를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | 표 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 표 추출이 지원되지 않을 경우 null이며, [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 객체의 컬렉션입니다.

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


문서에서 표를 자동으로 감지하여 추출합니다.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 표 추출이 지원되지 않을 경우 null이며, [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 객체의 컬렉션입니다.

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


문서 페이지에서 표를 추출합니다.

다음 예제는 문서 페이지에서 표를 추출하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | 표 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 표 추출이 지원되지 않을 경우 null이며, [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 객체의 컬렉션입니다.

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


문서 페이지에서 표를 자동으로 감지하여 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 0부터 시작하는 페이지 인덱스. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - 표 추출이 지원되지 않을 경우 null이며, [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 객체의 컬렉션입니다.

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


문서를 위한 조정 [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s를 생성합니다.

C#의 Java 구현
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (커밋 d4e691b /
ae9e98c). 사용자가 이후에 다듬거나 이름을 바꿀 수 있는 시작 템플릿으로 유용합니다.

### Algorithm

1. options.getPageIndex()에서 페이지를 선택합니다 (기본값 0).
2. 문서가 텍스트 영역 추출을 지원하는 경우, #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions)를 호출하고 비어 있지 않은 텍스트 영역마다 하나의 [TemplateField](../../com.groupdocs.parser.templates/templatefield)를 생성합니다. 이름은 {prefix}_{n} (기본 접두사 "Field")입니다. 각 필드는 텍스트 영역의 사각형에 [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)를 할당받으며, 페이지 너비는 pageWidth에 기록되어 이후 템플릿 스케일링에 사용됩니다.
3. 문서가 텍스트 영역을 지원하지 않으면 null을 반환합니다.

### OCR caveat

C# 구현은 문서가 이미지 전용인 경우 페이지 미리보기에 OCR을 실행하여 필드를 도출합니다. Java의 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase)는 사용자가 제공하므로, OCR 기반 생성은 커넥터가 구성되고 커넥터의 recognizeTextAreas(...)가 올바른 사각형을 반환할 때만 의미가 있습니다. options.getOcrOptions()가 설정되고 커넥터가 사용 가능하면 OCR 파이프라인이 우선됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | 생성 옵션입니다. null일 수 있으며(기본값이 적용됩니다). |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - 생성된 [TemplateItem](../../com.groupdocs.parser.templates/templateitem)들의 반복 가능한 컬렉션이며, 이 문서 형식에서 지원되지 않으면 null입니다.

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


스프레드시트의 모든 워크시트에 대한 정보를 추출합니다.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - 스프레드시트의 모든 워크시트에 대한 정보를 포함하는 [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) 인스턴스 목록입니다.

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


워크시트에 대한 정보를 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | worksheetIndex | int | 워크시트의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


워크시트 셀을 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | worksheetIndex | int | 워크시트의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - 셀 데이터를 포함하는 [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) 인스턴스들의 컬렉션입니다.

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


사용자 지정 옵션을 사용하여 워크시트 셀을 추출합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | worksheetIndex | int | 워크시트의 0부터 시작하는 인덱스입니다. |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | 워크시트 추출 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - 셀 데이터를 포함하는 [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) 인스턴스들의 컬렉션입니다.

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


사용자 생성 템플릿으로 문서를 구문 분석합니다.

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | 사용자 생성 템플릿입니다. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


제공된 옵션과 함께 사용자 생성 템플릿으로 문서를 구문 분석합니다.

만약
options.getPageIndex()
설정되면 해당 페이지만 파싱되고, 그렇지 않으면 모든 페이지가 파싱됩니다.

OCR 지원은 [ParserSettings](../../com.groupdocs.parser.options/parsersettings)에서 구성된 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase)에 따라 달라집니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | 사용자 생성 템플릿입니다. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | 템플릿 기반 파싱 옵션입니다. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


컬렉션에서 가장 일치하는 템플릿을 자동으로 선택하여 문서를 구문 분석합니다.

C#의 미러
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
커밋 71f3f21에서 도입되었습니다.

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), 그리고 생성되는 템플릿
가장 많은 채워진 필드(null이 아닌 페이지 영역에 비어 있지 않은 텍스트)가 승리합니다. C# 구현은 사용합니다
숨겨진 마커와 OCR 패스를 매칭하지만; 해당 경로는 아직 Java에서 제공되지 않으며, 숨겨진 필드 마커와
OCR 기반 TemplatePageOcrParser가 포팅되지 않아, 이 채워진 필드 수가 투명한 대체 수단으로 사용됩니다.
C#와 동일한 동작이 필요한 호출자는 OCR 엔진이 연결된 후 사용자 정의 셀렉터를 삽입해야 합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | 후보 템플릿의 컬렉션입니다. 파서는 가장 일치하는 템플릿을 선택합니다. |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | 구문 분석 옵션입니다. null 일 수 있습니다. |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


문서 양식을 구문 분석합니다.

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

다음 예제는 문서의 양식을 구문 분석하는 방법을 보여줍니다:

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


문서에서 구조화된 텍스트를 추출합니다.

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - XML 텍스트 구조를 가진 org.w3c.dom.Document 클래스의 인스턴스; 텍스트 구조 추출이 지원되지 않으면 null.

### close() {#close--}
```
public void close()
```


이 리소스를 닫고, 모든 기본 리소스를 해제합니다.


