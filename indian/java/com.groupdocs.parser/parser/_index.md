---
title: "Parser"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "मुख्य क्लास को दर्शाता है जो टेक्स्ट इमेज कंटेनर एक्सट्रैक्शन और पार्सिंग कार्यक्षमता को नियंत्रित करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.parser/parser/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Parser implements Closeable
```

मुख्य क्लास का प्रतिनिधित्व करता है जो टेक्स्ट, इमेज, कंटेनर निष्कर्षण और पार्सिंग कार्यक्षमता को नियंत्रित करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Parser(URL url)](#Parser-java.net.URL-) | एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए। |
|
|  | [Parser(URL url, LoadOptions loadOptions)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-) | एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए loadOptions के साथ। |
|
|  | [Parser(URL url, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-) | एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए parserSettings के साथ। |
|
|  | [Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए loadOptions और parserSettings के साथ। |
|
|  | [Parser(Connection connection)](#Parser-java.sql.Connection-) | डेटाबेस से डेटा निकालने के लिए [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(Connection connection, ParserSettings parserSettings)](#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-) | डेटाबेस से डेटा निकालने के लिए [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(EmailConnection connection)](#Parser-com.groupdocs.parser.options.EmailConnection-) | [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(EmailConnection connection, ParserSettings parserSettings)](#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-) | [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(String filePath)](#Parser-java.lang.String-) | [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(String filePath, LoadOptions loadOptions)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(String filePath, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-) | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) और [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(InputStream document)](#Parser-java.io.InputStream-) | [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(InputStream document, LoadOptions loadOptions)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(InputStream document, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-) | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)](#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) और [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileInfo(String filePath)](#getFileInfo-java.lang.String-) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
|
|  | [getFileInfo(InputStream document)](#getFileInfo-java.io.InputStream-) | फ़ाइल के बारे में सामान्य जानकारी लौटाता है। |
|
|  | [getFeatures()](#getFeatures--) | समर्थित विशेषताएँ प्राप्त करता है। |
|
|  | [getPagePreview(int pageIndex)](#getPagePreview-int-) | दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है। |
|
|  | [getPagePreview(int pageIndex, PagePreviewOptions options)](#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-) | अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है। |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.parser.options.PreviewOptions-) | पृष्ठों का पूर्वावलोकन प्राप्त करें। |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है। |
|
|  | [getText()](#getText--) | दस्तावेज़ से पाठ निकालता है। |
|
|  | [getText(TextOptions options)](#getText-com.groupdocs.parser.options.TextOptions-) | पाठ विकल्पों का उपयोग करके दस्तावेज़ से एक पाठ पृष्ठ निकालता है (कच्ची तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)। |
|
|  | [getText(int pageIndex)](#getText-int-) | दस्तावेज़ पृष्ठ से पाठ निकालता है। |
|
|  | [getText(int pageIndex, TextOptions options)](#getText-int-com.groupdocs.parser.options.TextOptions-) | पाठ विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से पाठ निकालता है (कच्ची तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)। |
|
|  | [getFormattedText(FormattedTextOptions options)](#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-) | दस्तावेज़ से स्वरूपित पाठ निकालता है। |
|
|  | [getFormattedText(int pageIndex, FormattedTextOptions options)](#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-) | दस्तावेज़ पृष्ठ से स्वरूपित पाठ निकालता है। |
|
|  | [search(String keyword)](#search-java.lang.String-) | दस्तावेज़ में एक कुंजीशब्द खोजता है। |
|
|  | [search(String keyword, SearchOptions options)](#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-) | खोज विकल्पों (नियमित अभिव्यक्ति, केस मिलान, आदि) का उपयोग करके दस्तावेज़ में एक कुंजीशब्द खोजता है। |
|
|  | [getHighlight(int position, boolean isDirect, HighlightOptions options)](#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-) | दस्तावेज़ से हाइलाइट निकालता है। |
|
|  | [getToc()](#getToc--) | दस्तावेज़ से सामग्री तालिका निकालता है। |
|
|  | [getMetadata()](#getMetadata--) | दस्तावेज़ से मेटाडेटा निकालता है। |
|
|  | [getAnnotations()](#getAnnotations--) | दस्तावेज़ से एनोटेशन निकालता है। |
|
|  | [getAnnotations(int pageIndex)](#getAnnotations-int-) | दस्तावेज़ पृष्ठ से एनोटेशन निकालता है। |
|
|  | [getContainer()](#getContainer--) | संलग्नक, ZIP अभिलेख आदि वाले फ़ॉर्मेट्स के साथ काम करने के लिए दस्तावेज़ से एक कंटेनर ऑब्जेक्ट निकालता है। |
|
|  | [getTextAreas()](#getTextAreas--) | दस्तावेज़ से टेक्स्ट क्षेत्रों को निकालता है। |
|
|  | [getTextAreas(PageTextAreaOptions options)](#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-) | दस्तावेज़ से टेक्स्ट क्षेत्रों को अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, केस मिलान, आदि) का उपयोग करके निकालता है। |
|
|  | [getTextAreas(int pageIndex)](#getTextAreas-int-) | दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्रों को निकालता है। |
|
|  | [getTextAreas(int pageIndex, PageTextAreaOptions options)](#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-) | दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्रों को अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, केस मिलान, आदि) का उपयोग करके निकालता है। |
|
|  | [getImages()](#getImages--) | दस्तावेज़ से छवियों को निकालता है। |
|
|  | [getImages(PageAreaOptions options)](#getImages-com.groupdocs.parser.options.PageAreaOptions-) | दस्तावेज़ से छवियों को अनुकूलन विकल्पों (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है। |
|
|  | [getImages(int pageIndex)](#getImages-int-) | दस्तावेज़ पृष्ठ से छवियों को निकालता है। |
|
|  | [getImages(int pageIndex, PageAreaOptions options)](#getImages-int-com.groupdocs.parser.options.PageAreaOptions-) | दस्तावेज़ पृष्ठ से छवियों को अनुकूलन विकल्पों (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है। |
|
|  | [getHyperlinks()](#getHyperlinks--) | दस्तावेज़ से हाइपरलिंक को निकालता है। |
|
|  | [getHyperlinks(int pageIndex)](#getHyperlinks-int-) | दस्तावेज़ पृष्ठ से हाइपरलिंक को निकालता है। |
|
|  | [getHyperlinks(PageAreaOptions options)](#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-) | दस्तावेज़ से हाइपरलिंक को अनुकूलन विकल्पों (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है। |
|
|  | [getHyperlinks(int pageIndex, PageAreaOptions options)](#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-) | दस्तावेज़ पृष्ठ से हाइपरलिंक को अनुकूलन विकल्पों (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है। |
|
|  | [getBarcodes()](#getBarcodes--) | दस्तावेज़ से बारकोड को निकालता है। |
|
|  | [getBarcodes(int pageIndex)](#getBarcodes-int-) | दस्तावेज़ पृष्ठ से बारकोड को निकालता है। |
|
|  | [getBarcodes(BarcodeOptions options)](#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-) | दस्तावेज़ से बारकोड को अनुकूलन विकल्पों (बारकोड वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है। |
|
|  | [getBarcodes(int pageIndex, BarcodeOptions options)](#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-) | दस्तावेज़ पृष्ठ से बारकोड को अनुकूलन विकल्पों (बारकोड वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है। |
|
|  | [getTables(PageTableAreaOptions options)](#getTables-com.groupdocs.parser.options.PageTableAreaOptions-) | दस्तावेज़ से तालिकाओं को निकालता है। |
|
|  | [getTables()](#getTables--) | दस्तावेज़ से तालिकाओं को निकालता है, उन्हें स्वचालित रूप से पहचानते हुए। |
|
|  | [getTables(int pageIndex, PageTableAreaOptions options)](#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-) | दस्तावेज़ पृष्ठ से तालिकाओं को निकालता है। |
|
|  | [getTables(int pageIndex)](#getTables-int-) | दस्तावेज़ पृष्ठ से तालिकाओं को निकालता है, उन्हें स्वचालित रूप से पहचानते हुए। |
|
|  | [generateAdjustmentFields(GenerateTemplateOptions options)](#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-) | दस्तावेज़ के लिए समायोजन [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s का संग्रह उत्पन्न करता है। |
|
|  | [getWorksheetInfo()](#getWorksheetInfo--) | स्प्रेडशीट में सभी कार्यपत्रकों की जानकारी निकालता है। |
|
|  | [getWorksheetInfo(int worksheetIndex)](#getWorksheetInfo-int-) | कार्यपत्रक की जानकारी निकालता है। |
|
|  | [getWorksheetCells(int worksheetIndex)](#getWorksheetCells-int-) | कार्यपत्रक की कोशिकाओं को निकालता है। |
|
|  | [getWorksheetCells(int worksheetIndex, WorksheetOptions options)](#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-) | कार्यपत्रक की कोशिकाओं को अनुकूलन विकल्पों का उपयोग करके निकालता है। |
|
|  | [parseByTemplate(Template template)](#parseByTemplate-com.groupdocs.parser.templates.Template-) | उपयोगकर्ता-जनित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है। |
|
|  | [parseByTemplate(Template template, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-) | प्रदान किए गए विकल्पों के साथ उपयोगकर्ता-जनित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है। |
|
|  | [parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)](#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-) | संग्रह से सबसे उपयुक्त टेम्पलेट को स्वचालित रूप से चुनकर दस्तावेज़ को पार्स करता है। |
|
|  | [parseForm()](#parseForm--) | दस्तावेज़ फ़ॉर्म को पार्स करता है। |
|
|  | [getStructure()](#getStructure--) | दस्तावेज़ से संरचित पाठ निकालता है। |
|
|  | [close()](#close--) | इस संसाधन को बंद करता है, सभी अंतर्निहित संसाधनों को मुक्त करता है। |
|
### Parser(URL url) {#Parser-java.net.URL-}
```
public Parser(URL url)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | url | java.net.URL | वह URL जहाँ अनुरोध भेजा जाता है |
|

### Parser(URL url, LoadOptions loadOptions) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(URL url, LoadOptions loadOptions)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए loadOptions के साथ।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | url | java.net.URL | वह URL जहाँ अनुरोध भेजा जाता है। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | फ़ाइल खोलने के विकल्प। |
|

### Parser(URL url, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, ParserSettings parserSettings)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए parserSettings के साथ।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | url | java.net.URL | वह URL जहाँ अनुरोध भेजा जाता है। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.net.URL-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(URL url, LoadOptions loadOptions, ParserSettings parserSettings)
```


एक नया इंस्टेंस इनिशियलाइज़ करता है [Parser](../../com.groupdocs.parser/parser) क्लास का URL से डेटा निकालने के लिए loadOptions और parserSettings के साथ।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | url | java.net.URL | वह URL जहाँ अनुरोध भेजा जाता है। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | फ़ाइल खोलने के विकल्प। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(Connection connection) {#Parser-java.sql.Connection-}
```
public Parser(Connection connection)
```


डेटाबेस से डेटा निकालने के लिए [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)

निम्न उदाहरण दिखाता है कि Sqlite डेटाबेस से डेटा कैसे निकाला जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कनेक्शन | java.sql.Connection | डेटाबेस कनेक्शन। |
|

### Parser(Connection connection, ParserSettings parserSettings) {#Parser-java.sql.Connection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(Connection connection, ParserSettings parserSettings)
```


डेटाबेस से डेटा निकालने के लिए [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Extract data from databases](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+databases)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

निम्न उदाहरण दिखाता है कि Sqlite डेटाबेस से डेटा कैसे निकाला जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कनेक्शन | java.sql.Connection | डेटाबेस कनेक्शन। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(EmailConnection connection) {#Parser-com.groupdocs.parser.options.EmailConnection-}
```
public Parser(EmailConnection connection)
```


[Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

निम्न उदाहरण दिखाता है कि Exchange Server से ईमेल कैसे निकाले जाएँ:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | ईमेल कनेक्शन। |
|

### Parser(EmailConnection connection, ParserSettings parserSettings) {#Parser-com.groupdocs.parser.options.EmailConnection-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(EmailConnection connection, ParserSettings parserSettings)
```


[Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

निम्न उदाहरण दिखाता है कि Exchange Server से ईमेल कैसे निकाले जाएँ:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | connection | [EmailConnection](../../com.groupdocs.parser.options/emailconnection) | ईमेल कनेक्शन। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(String filePath) {#Parser-java.lang.String-}
```
public Parser(String filePath)
```


[Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)

निम्न उदाहरण दिखाता है कि स्थानीय डिस्क से दस्तावेज़ कैसे लोड किया जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|

### Parser(String filePath, LoadOptions loadOptions) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(String filePath, LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

दस्तावेज़ पासवर्ड को [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास द्वारा पास किया जाता है:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | फ़ाइल खोलने के विकल्प। |
|

### Parser(String filePath, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, ParserSettings parserSettings)
```


[ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.lang.String-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(String filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) और [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Load document from local disk](../https://docs.groupdocs.com/display/parserjava/Load+document+from+local+disk)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

निम्न उदाहरण दिखाता है कि जानकारी को [ILogger](../../com.groupdocs.parser.options/ilogger) इंटरफ़ेस के माध्यम से कैसे प्राप्त किया जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | फ़ाइल खोलने के विकल्प। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(InputStream document) {#Parser-java.io.InputStream-}
```
public Parser(InputStream document)
```


[Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)

निम्न उदाहरण दिखाता है कि स्ट्रीम से दस्तावेज़ कैसे लोड किया जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|

### Parser(InputStream document, LoadOptions loadOptions) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-}
```
public Parser(InputStream document, LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

कुछ मामलों में [FileFormat](../../com.groupdocs.parser.options/fileformat) को परिभाषित करना आवश्यक होता है। विशेष मामलों (डेटाबेस, ईमेल सर्वर) के लिए भी
और सामग्री के आधार पर फ़ाइल प्रकार का पता लगाने के लिए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | फ़ाइल खोलने के विकल्प। |
|

### Parser(InputStream document, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, ParserSettings parserSettings)
```


[ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings) {#Parser-java.io.InputStream-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public Parser(InputStream document, LoadOptions loadOptions, ParserSettings parserSettings)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) और [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ [Parser](../../com.groupdocs.parser/parser) क्लास का नया उदाहरण प्रारंभ करता है।

**Learn more:**

* [Load document from stream](../https://docs.groupdocs.com/display/parserjava/Load+document+from+stream)
* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)
* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

निम्न उदाहरण दिखाता है कि जानकारी को [ILogger](../../com.groupdocs.parser.options/ilogger) इंटरफ़ेस के माध्यम से कैसे प्राप्त किया जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | फ़ाइल खोलने के विकल्प। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

### getFileInfo(String filePath) {#getFileInfo-java.lang.String-}
```
public static FileInfo getFileInfo(String filePath)
```


फ़ाइल के बारे में सामान्य जानकारी लौटाता है।

निम्न कोड दिखाता है कि फ़ाइल पासवर्ड-प्रोटेक्टेड है या नहीं, इसे कैसे जांचें:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFileInfo(InputStream document) {#getFileInfo-java.io.InputStream-}
```
public static FileInfo getFileInfo(InputStream document)
```


फ़ाइल के बारे में सामान्य जानकारी लौटाता है।

निम्न कोड दिखाता है कि फ़ाइल पासवर्ड-प्रोटेक्टेड है या नहीं, इसे कैसे जांचें:

````
// Get a file info
 FileInfo info = Parser.getFileInfo(filePath);
 // Check IsEncrypted property
 System.out.println(info.isEncrypted() ? "Password is required" : "");
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़ | java.io.InputStream | स्रोत इनपुट स्ट्रीम। |
|

**Returns:**
[FileInfo](../../com.groupdocs.parser.options/fileinfo) - An instance of [FileInfo](../../com.groupdocs.parser.options/fileinfo) class.

### getFeatures() {#getFeatures--}
```
public Features getFeatures()
```


समर्थित विशेषताएँ प्राप्त करता है।

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

यदि फीचर समर्थित नहीं है, तो मेथड लौटाता है
null
मान के बजाय। कुछ ऑपरेशन्स उपभोग कर सकते हैं
महत्वपूर्ण समय। इसलिए फीचर के समर्थन की जाँच करने के लिए केवल मेथड को कॉल करना अनुकूल नहीं है।
इस उद्देश्य के लिए Features प्रॉपर्टी का उपयोग किया जाता है:

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


दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.io.OutputStream - java.io.OutputStream का एक इंस्टेंस जिसमें दस्तावेज़ पृष्ठ की छवि होती है; यदि पृष्ठ प्रीव्यू जनरेशन समर्थित नहीं है तो null।

### getPagePreview(int pageIndex, PagePreviewOptions options) {#getPagePreview-int-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OutputStream getPagePreview(int pageIndex, PagePreviewOptions options)
```


अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | प्रीव्यू जनरेशन को कस्टमाइज़ करने के विकल्प। |
|

**Returns:**
java.io.OutputStream - java.io.OutputStream का एक इंस्टेंस जिसमें दस्तावेज़ पृष्ठ की छवि होती है; यदि पृष्ठ प्रीव्यू जनरेशन समर्थित नहीं है तो null।

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.parser.options.PreviewOptions-}
```
public void generatePreview(PreviewOptions previewOptions)
```


पृष्ठों का पूर्वावलोकन प्राप्त करें।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) | प्रीव्यू जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट्स सेट करने के विकल्प। |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public IDocumentInfo getDocumentInfo()
```


दस्तावेज़ के बारे में सामान्य जानकारी लौटाता है।

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ जानकारी कैसे प्राप्त करें:

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


दस्तावेज़ से पाठ निकालता है।

**Learn more:**

* [Extract text from documents](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+documents)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ से टेक्स्ट कैसे निकालें:

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


पाठ विकल्पों का उपयोग करके दस्तावेज़ से एक पाठ पृष्ठ निकालता है (कच्ची तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)।

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ से रॉ टेक्स्ट कैसे निकालें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | टेक्स्ट एक्सट्रैक्शन विकल्प। |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text extraction isn't supported.

### getText(int pageIndex) {#getText-int-}
```
public TextReader getText(int pageIndex)
```


दस्तावेज़ पृष्ठ से पाठ निकालता है।

**Learn more:**

* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से टेक्स्ट कैसे निकालें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getText(int pageIndex, TextOptions options) {#getText-int-com.groupdocs.parser.options.TextOptions-}
```
public TextReader getText(int pageIndex, TextOptions options)
```


पाठ विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से पाठ निकालता है (कच्ची तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)।

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से रॉ टेक्स्ट कैसे निकालें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [TextOptions](../../com.groupdocs.parser.options/textoptions) | टेक्स्ट एक्सट्रैक्शन विकल्प। |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if text page extraction isn't supported.

### getFormattedText(FormattedTextOptions options) {#getFormattedText-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(FormattedTextOptions options)
```


दस्तावेज़ से स्वरूपित पाठ निकालता है।

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ टेक्स्ट को HTML टेक्स्ट के रूप में कैसे निकालें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | फ़ॉर्मेटेड टेक्स्ट एक्सट्रैक्शन विकल्प। |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text extraction isn't supported.

### getFormattedText(int pageIndex, FormattedTextOptions options) {#getFormattedText-int-com.groupdocs.parser.options.FormattedTextOptions-}
```
public TextReader getFormattedText(int pageIndex, FormattedTextOptions options)
```


दस्तावेज़ पृष्ठ से स्वरूपित पाठ निकालता है।

**Learn more:**

* [Extract formatted text from document page](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ टेक्स्ट को मार्कडाउन टेक्स्ट के रूप में कैसे निकालें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) | फ़ॉर्मेटेड टेक्स्ट एक्सट्रैक्शन विकल्प। |
|

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text;  null  if formatted text page extraction isn't supported.

### search(String keyword) {#search-java.lang.String-}
```
public Iterable<SearchResult> search(String keyword)
```


दस्तावेज़ में एक कुंजीशब्द खोजता है।

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

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ में कीवर्ड कैसे खोजें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कीवर्ड | java.lang.String | खोजने के लिए कीवर्ड। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) ऑब्जेक्ट्स का एक संग्रह; यदि सर्च समर्थित नहीं है तो null।

### search(String keyword, SearchOptions options) {#search-java.lang.String-com.groupdocs.parser.options.SearchOptions-}
```
public Iterable<SearchResult> search(String keyword, SearchOptions options)
```


खोज विकल्पों (नियमित अभिव्यक्ति, केस मिलान, आदि) का उपयोग करके दस्तावेज़ में एक कुंजीशब्द खोजता है।

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

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ में रेगुलर एक्सप्रेशन के साथ कैसे सर्च करें:

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

निम्नलिखित उदाहरण दिखाता है कि पृष्ठों पर टेक्स्ट कैसे सर्च करें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कीवर्ड | java.lang.String | खोजने के लिए कीवर्ड। |
|
|  | options | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) | सर्च विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.SearchResult> - [SearchResult](../../com.groupdocs.parser.data/searchresult) ऑब्जेक्ट्स का एक संग्रह; यदि सर्च समर्थित नहीं है तो null।

### getHighlight(int position, boolean isDirect, HighlightOptions options) {#getHighlight-int-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public HighlightItem getHighlight(int position, boolean isDirect, HighlightOptions options)
```


दस्तावेज़ से हाइलाइट निकालता है।

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

निम्नलिखित उदाहरण दिखाता है कि 3 शब्दों वाला हाइलाइट कैसे निकालें:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्थिति | int | हाइलाइट की प्रारंभिक स्थिति। |
|
|  | isDirect | boolean | वह मान जो दर्शाता है कि हाइलाइट निष्कर्षण प्रत्यक्ष है या नहीं।  true  यदि हाइलाइट स्थिति के दाएँ से निकाला जाता है; अन्यथा,  false . |
|
|  | options | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | हाइलाइट निष्कर्षण विकल्प। |
|

**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class that represents the extracted highlight;  null  if highlight extraction isn't supported.

### getToc() {#getToc--}
```
public Iterable<TocItem> getToc()
```


दस्तावेज़ से सामग्री तालिका निकालता है।

**Learn more:**

* [Extract table of contents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents)
* [Extract text by table of contents item](../https://docs.groupdocs.com/display/parserjava/Extract+text+by+table+of+contents+item)
* [Extract table of contents from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [Extract table of contents from EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Extract+table+of+contents+from+EPUB+eBooks)

निम्न उदाहरण दिखाता है कि EPUB फ़ाइल से सामग्री तालिका कैसे निकाली जाए:

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
java.lang.Iterable<com.groupdocs.parser.data.TocItem> - सामग्री तालिका आइटम्स का संग्रह;  null  यदि सामग्री तालिका निष्कर्षण समर्थित नहीं है।

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


दस्तावेज़ से मेटाडेटा निकालता है।

**Learn more:**

* [Extract metadata from documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+documents)
* [Extract metadata from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Extract metadata from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Extract metadata from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [Extract metadata from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+PDF+documents)
* [Extract metadata from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+metadata+from+Emails)

निम्न उदाहरण दिखाता है कि दस्तावेज़ से मेटाडेटा कैसे निकाला जाए:

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
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - मेटाडेटा आइटम्स का संग्रह;  null  यदि मेटाडेटा निष्कर्षण समर्थित नहीं है।

### getAnnotations() {#getAnnotations--}
```
public Iterable<AnnotationItem> getAnnotations()
```


दस्तावेज़ से एनोटेशन निकालता है।


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - एनोटेशन आइटम्स का संग्रह;  null  यदि एनोटेशन निष्कर्षण समर्थित नहीं है।

### getAnnotations(int pageIndex) {#getAnnotations-int-}
```
public Iterable<AnnotationItem> getAnnotations(int pageIndex)
```


दस्तावेज़ पृष्ठ से एनोटेशन निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.AnnotationItem> - एनोटेशन आइटम्स का संग्रह;  null  यदि एनोटेशन निष्कर्षण समर्थित नहीं है।

### getContainer() {#getContainer--}
```
public Iterable<ContainerItem> getContainer()
```


संलग्नक, ZIP अभिलेख आदि वाले फ़ॉर्मेट्स के साथ काम करने के लिए दस्तावेज़ से एक कंटेनर ऑब्जेक्ट निकालता है।

**Learn more:**

* [Extract data from attachments and ZIP archives](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](../https://docs.groupdocs.com/display/parserjava/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](../https://docs.groupdocs.com/display/parserjava/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](../https://docs.groupdocs.com/display/parserjava/Extract+text+from+ZIP+archive+files)

निम्न उदाहरण दिखाता है कि ज़िप इकाइयों से टेक्स्ट कैसे निकाला जाए:

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
java.lang.Iterable<com.groupdocs.parser.data.ContainerItem> - कंटेनर आइटम्स का संग्रह;  null  यदि कंटेनर निष्कर्षण समर्थित नहीं है।

### getTextAreas() {#getTextAreas--}
```
public Iterable<PageTextArea> getTextAreas()
```


दस्तावेज़ से टेक्स्ट क्षेत्रों को निकालता है।

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

निम्न उदाहरण दिखाता है कि पूरे दस्तावेज़ से सभी टेक्स्ट क्षेत्रों को कैसे निकाला जाए:

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
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह;  null  यदि टेक्स्ट क्षेत्रों का निष्कर्षण समर्थित नहीं है।

### getTextAreas(PageTextAreaOptions options) {#getTextAreas-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(PageTextAreaOptions options)
```


दस्तावेज़ से टेक्स्ट क्षेत्रों को अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, केस मिलान, आदि) का उपयोग करके निकालता है।

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

निम्न उदाहरण दिखाता है कि ऊपरी-बाएँ courner से केवल अंकों वाले टेक्स्ट क्षेत्रों को कैसे निकाला जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | टेक्स्ट क्षेत्र निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह;  null  यदि टेक्स्ट क्षेत्रों का निष्कर्षण समर्थित नहीं है।

### getTextAreas(int pageIndex) {#getTextAreas-int-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex)
```


दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्रों को निकालता है।

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्रों को निकालने के लिए निम्न विधि का उपयोग किया जाता है:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह;  null  यदि टेक्स्ट क्षेत्रों का निष्कर्षण समर्थित नहीं है।

### getTextAreas(int pageIndex, PageTextAreaOptions options) {#getTextAreas-int-com.groupdocs.parser.options.PageTextAreaOptions-}
```
public Iterable<PageTextArea> getTextAreas(int pageIndex, PageTextAreaOptions options)
```


दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्रों को अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, केस मिलान, आदि) का उपयोग करके निकालता है।

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) | टेक्स्ट क्षेत्र निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह;  null  यदि टेक्स्ट क्षेत्रों का निष्कर्षण समर्थित नहीं है।

### getImages() {#getImages--}
```
public Iterable<PageImageArea> getImages()
```


दस्तावेज़ से छवियों को निकालता है।

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

निम्न उदाहरण दिखाता है कि पूरे दस्तावेज़ से सभी छवियों को कैसे निकाला जाए:

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
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स का संग्रह;  null  यदि छवियों का निष्कर्षण समर्थित नहीं है।

### getImages(PageAreaOptions options) {#getImages-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(PageAreaOptions options)
```


दस्तावेज़ से छवियों को अनुकूलन विकल्पों (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है।

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

निम्न उदाहरण दिखाता है कि ऊपरी-बाएँ courner से केवल छवियों को कैसे निकाला जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | छवियों के निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स का संग्रह;  null  यदि छवियों का निष्कर्षण समर्थित नहीं है।

### getImages(int pageIndex) {#getImages-int-}
```
public Iterable<PageImageArea> getImages(int pageIndex)
```


दस्तावेज़ पृष्ठ से छवियों को निकालता है।

**Learn more:**

* [Extract images from documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+documents)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)
* [Extract images from document page](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+Emails)
* [Extract images from PDF documents](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+PDF+documents)

दस्तावेज़ पृष्ठ से छवियों को निकालने के लिए निम्न विधि का उपयोग किया जाता है:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स का संग्रह;  null  यदि छवियों का निष्कर्षण समर्थित नहीं है।

### getImages(int pageIndex, PageAreaOptions options) {#getImages-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageImageArea> getImages(int pageIndex, PageAreaOptions options)
```


दस्तावेज़ पृष्ठ से छवियों को अनुकूलन विकल्पों (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है।

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | छवियों के निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageImageArea> - [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स का संग्रह;  null  यदि छवियों का निष्कर्षण समर्थित नहीं है।

### getHyperlinks() {#getHyperlinks--}
```
public Iterable<PageHyperlinkArea> getHyperlinks()
```


दस्तावेज़ से हाइपरलिंक को निकालता है।

निम्न उदाहरण दिखाता है कि पूरे दस्तावेज़ से सभी हाइपरलिंक को कैसे निकाला जाए:

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
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का संग्रह;  null  यदि हाइपरलिंक का निष्कर्षण समर्थित नहीं है।

### getHyperlinks(int pageIndex) {#getHyperlinks-int-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex)
```


दस्तावेज़ पृष्ठ से हाइपरलिंक को निकालता है।

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से हाइपरलिंक को कैसे निकाला जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का संग्रह;  null  यदि हाइपरलिंक का निष्कर्षण समर्थित नहीं है।

### getHyperlinks(PageAreaOptions options) {#getHyperlinks-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(PageAreaOptions options)
```


दस्तावेज़ से हाइपरलिंक को अनुकूलन विकल्पों (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है।

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक को कैसे निकाला जाए:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | हाइपरलिंक निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का संग्रह;  null  यदि हाइपरलिंक का निष्कर्षण समर्थित नहीं है।

### getHyperlinks(int pageIndex, PageAreaOptions options) {#getHyperlinks-int-com.groupdocs.parser.options.PageAreaOptions-}
```
public Iterable<PageHyperlinkArea> getHyperlinks(int pageIndex, PageAreaOptions options)
```


दस्तावेज़ पृष्ठ से हाइपरलिंक को अनुकूलन विकल्पों (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है।

निम्न उदाहरण दिखाता है कि कैसे कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक निकाले जाएँ:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) | हाइपरलिंक निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageHyperlinkArea> - [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का संग्रह;  null  यदि हाइपरलिंक का निष्कर्षण समर्थित नहीं है।

### getBarcodes() {#getBarcodes--}
```
public Iterable<PageBarcodeArea> getBarcodes()
```


दस्तावेज़ से बारकोड को निकालता है।


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - एक संग्रह है [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का;  null  यदि बारकोड निष्कर्षण समर्थित नहीं है।

### getBarcodes(int pageIndex) {#getBarcodes-int-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex)
```


दस्तावेज़ पृष्ठ से बारकोड को निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - एक संग्रह है [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का;  null  यदि बारकोड निष्कर्षण समर्थित नहीं है।

### getBarcodes(BarcodeOptions options) {#getBarcodes-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(BarcodeOptions options)
```


दस्तावेज़ से बारकोड को अनुकूलन विकल्पों (बारकोड वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | बारकोड निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - एक संग्रह है [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का;  null  यदि बारकोड निष्कर्षण समर्थित नहीं है।\\

### getBarcodes(int pageIndex, BarcodeOptions options) {#getBarcodes-int-com.groupdocs.parser.options.BarcodeOptions-}
```
public Iterable<PageBarcodeArea> getBarcodes(int pageIndex, BarcodeOptions options)
```


दस्तावेज़ पृष्ठ से बारकोड को अनुकूलन विकल्पों (बारकोड वाले आयताकार क्षेत्र को सेट करने के लिए) का उपयोग करके निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [BarcodeOptions](../../com.groupdocs.parser.options/barcodeoptions) | बारकोड निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> - एक संग्रह है [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का;  null  यदि बारकोड निष्कर्षण समर्थित नहीं है।

### getTables(PageTableAreaOptions options) {#getTables-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(PageTableAreaOptions options)
```


दस्तावेज़ से तालिकाओं को निकालता है।

निम्न उदाहरण दिखाता है कि पूरे दस्तावेज़ से तालिकाएँ कैसे निकाली जाएँ:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | तालिका निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - एक संग्रह है [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का;  null  यदि तालिका निष्कर्षण समर्थित नहीं है।

### getTables() {#getTables--}
```
public Iterable<PageTableArea> getTables()
```


दस्तावेज़ से तालिकाओं को निकालता है, उन्हें स्वचालित रूप से पहचानते हुए।


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - एक संग्रह है [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का;  null  यदि तालिका निष्कर्षण समर्थित नहीं है।

### getTables(int pageIndex, PageTableAreaOptions options) {#getTables-int-com.groupdocs.parser.options.PageTableAreaOptions-}
```
public Iterable<PageTableArea> getTables(int pageIndex, PageTableAreaOptions options)
```


दस्तावेज़ पृष्ठ से तालिकाओं को निकालता है।

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से तालिकाएँ कैसे निकाली जाएँ:

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | options | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) | तालिका निष्कर्षण के विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - एक संग्रह है [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का;  null  यदि तालिका निष्कर्षण समर्थित नहीं है।

### getTables(int pageIndex) {#getTables-int-}
```
public Iterable<PageTableArea> getTables(int pageIndex)
```


दस्तावेज़ पृष्ठ से तालिकाओं को निकालता है, उन्हें स्वचालित रूप से पहचानते हुए।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> - एक संग्रह है [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का;  null  यदि तालिका निष्कर्षण समर्थित नहीं है।

### generateAdjustmentFields(GenerateTemplateOptions options) {#generateAdjustmentFields-com.groupdocs.parser.options.GenerateTemplateOptions-}
```
public Iterable<TemplateItem> generateAdjustmentFields(GenerateTemplateOptions options)
```


दस्तावेज़ के लिए समायोजन [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s का संग्रह उत्पन्न करता है।

C# का जावा प्रतिबिंब
Parser.GenerateAdjustmentFields(GenerateTemplateOptions)
API (कमिट्स d4e691b /
ae9e98c). उपयोगी प्रारंभिक टेम्प्लेट के रूप में जिसे उपयोगकर्ता फिर संशोधित या पुनःनामित कर सकता है।

### Algorithm

1. पृष्ठ चुनें  options.getPageIndex()  से (डिफ़ॉल्ट  0 ).
2. यदि दस्तावेज़ टेक्स्ट-एरिया निष्कर्षण का समर्थन करता है, तो कॉल करें #getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions).getTextAreas(int, com.groupdocs.parser.options.PageTextAreaOptions) और प्रत्येक गैर-खाली टेक्स्ट एरिया के लिए एक [TemplateField](../../com.groupdocs.parser.templates/templatefield) उत्पन्न करें, जिसका नाम {prefix}_{n} (डिफ़ॉल्ट प्रीफ़िक्स "Field") है। प्रत्येक फ़ील्ड को टेक्स्ट एरिया के आयत में एक [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) मिलता है, पृष्ठ की चौड़ाई को pageWidth के रूप में रिकॉर्ड किया जाता है ताकि बाद में टेम्प्लेट स्केलिंग काम करे।
3. यदि दस्तावेज़ टेक्स्ट एरिया का समर्थन नहीं करता, तो  null  लौटाएँ।

### OCR caveat

C# कार्यान्वयन पृष्ठ पूर्वावलोकन पर OCR चलाता है ताकि जब दस्तावेज़ केवल छवि हो तो फ़ील्ड निकाले जा सकें। Java का [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) उपयोगकर्ता द्वारा प्रदान किया गया है, इसलिए OCR-आधारित जनरेशन केवल तभी सार्थक है जब एक कनेक्टर कॉन्फ़िगर किया गया हो और कनेक्टर का  recognizeTextAreas(...)  उचित आयतें लौटाए। जब  options.getOcrOptions()  सेट हो और एक कनेक्टर उपलब्ध हो, तो OCR पाइपलाइन को प्राथमिकता दी जाती है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [GenerateTemplateOptions](../../com.groupdocs.parser.options/generatetemplateoptions) | जनरेशन विकल्प। यह  null  हो सकता है (डिफ़ॉल्ट लागू)। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.templates.TemplateItem> - एक इटेरेबल है उत्पन्न किए गए [TemplateItem](../../com.groupdocs.parser.templates/templateitem)s का, या  null  यदि इस दस्तावेज़ फ़ॉर्मेट द्वारा समर्थित नहीं है।

### getWorksheetInfo() {#getWorksheetInfo--}
```
public Iterable<WorksheetInfo> getWorksheetInfo()
```


स्प्रेडशीट में सभी कार्यपत्रकों की जानकारी निकालता है।


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetInfo> - एक सूची है [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) इंस्टेंस की जो स्प्रेडशीट में सभी वर्कशीट्स की जानकारी रखती है।

### getWorksheetInfo(int worksheetIndex) {#getWorksheetInfo-int-}
```
public WorksheetInfo getWorksheetInfo(int worksheetIndex)
```


कार्यपत्रक की जानकारी निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | worksheetIndex | int | वर्कशीट का शून्य-आधारित सूचकांक। |
|

**Returns:**
[WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) - An instance of [WorksheetInfo](../../com.groupdocs.parser.data/worksheetinfo) that contains the info about the worksheet.

### getWorksheetCells(int worksheetIndex) {#getWorksheetCells-int-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex)
```


कार्यपत्रक की कोशिकाओं को निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | worksheetIndex | int | वर्कशीट का शून्य-आधारित सूचकांक। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - एक संग्रह है [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) इंस्टेंस का जो सेल डेटा रखता है।

### getWorksheetCells(int worksheetIndex, WorksheetOptions options) {#getWorksheetCells-int-com.groupdocs.parser.options.WorksheetOptions-}
```
public Iterable<WorksheetCell> getWorksheetCells(int worksheetIndex, WorksheetOptions options)
```


कार्यपत्रक की कोशिकाओं को अनुकूलन विकल्पों का उपयोग करके निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | worksheetIndex | int | वर्कशीट का शून्य-आधारित सूचकांक। |
|
|  | options | [WorksheetOptions](../../com.groupdocs.parser.options/worksheetoptions) | वर्कशीट निष्कर्षण विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.WorksheetCell> - एक संग्रह है [WorksheetCell](../../com.groupdocs.parser.data/worksheetcell) इंस्टेंस का जो सेल डेटा रखता है।

### parseByTemplate(Template template) {#parseByTemplate-com.groupdocs.parser.templates.Template-}
```
public DocumentData parseByTemplate(Template template)
```


उपयोगकर्ता-जनित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है।

**Learn more:**

* [Parse data from documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+documents)
* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | उपयोगकर्ता-जनित टेम्प्लेट। |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(Template template, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.Template-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(Template template, ParseByTemplateOptions options)
```


प्रदान किए गए विकल्पों के साथ उपयोगकर्ता-जनित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है।

यदि
options.getPageIndex()
सेट किया गया है, केवल वही पृष्ठ पार्स किया जाता है; अन्यथा सभी पृष्ठ पार्स किए जाते हैं।

OCR समर्थन इस पर निर्भर करता है कि [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) को [ParserSettings](../../com.groupdocs.parser.options/parsersettings) में कॉन्फ़िगर किया गया है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | template | [Template](../../com.groupdocs.parser.templates/template) | उपयोगकर्ता-जनित टेम्प्लेट। |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | पार्स-बाय-टेम्प्लेट विकल्प। |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - An instance of [DocumentData](../../com.groupdocs.parser.data/documentdata) class that contains the extracted data;  null  if parsing by template isn't supported.

### parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options) {#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection-com.groupdocs.parser.options.ParseByTemplateOptions-}
```
public DocumentData parseByTemplate(TemplateCollection templates, ParseByTemplateOptions options)
```


संग्रह से सबसे उपयुक्त टेम्पलेट को स्वचालित रूप से चुनकर दस्तावेज़ को पार्स करता है।

C# का प्रतिबिंब।
Parser.ParseByTemplate(TemplateCollection, ParseByTemplateOptions)
कमिट 71f3f21 में पेश किया गया।

**Selection heuristic** (Java port): each candidate template is applied via
#parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions).parseByTemplate(Template, com.groupdocs.parser.options.ParseByTemplateOptions), और वह टेम्प्लेट जो देता है
सबसे अधिक संख्या में भरे हुए फ़ील्ड (नॉन-नल पेज एरिया जिनमें खाली नहीं टेक्स्ट है) जीतते हैं। C# कार्यान्वयन उपयोग करता है
हिडन-मार्कर मिलान OCR पास के विरुद्ध; यह पाथ अभी तक जावा में उपलब्ध नहीं है क्योंकि हिडन-फ़ील्ड मार्कर और
OCR-ड्रिवेन TemplatePageOcrParser पोर्ट नहीं किए गए हैं, इसलिए यह भरे हुए फ़ील्ड काउंट को एक पारदर्शी फॉलबैक के रूप में उपयोग किया जाता है।
वे कॉलर जो C#-समान व्यवहार चाहते हैं, उन्हें OCR इंजन के जुड़े होने पर एक कस्टम सिलेक्टर प्लग इन करना चाहिए।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | templates | [TemplateCollection](../../com.groupdocs.parser.templates/templatecollection) | उम्मीदवार टेम्प्लेट्स का संग्रह। पार्सर सबसे उपयुक्त को चुनेगा। |
|
|  | options | [ParseByTemplateOptions](../../com.groupdocs.parser.options/parsebytemplateoptions) | पार्स विकल्प। null हो सकता है। |
|

**Returns:**
[DocumentData](../../com.groupdocs.parser.data/documentdata) - The extracted data with [DocumentData.getTemplate()](../../com.groupdocs.parser.data/documentdata#getTemplate--) set to the selected template, or  null  if the document does not support parsing-by-template or the collection is empty / produced no result.

### parseForm() {#parseForm--}
```
public DocumentData parseForm()
```


दस्तावेज़ फ़ॉर्म को पार्स करता है।

**Learn more:**

* [Extract data from PDF forms](../https://docs.groupdocs.com/display/parserjava/Extract+data+from+PDF+forms)
* [Working with data extracted by template](../https://docs.groupdocs.com/display/parserjava/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](../https://docs.groupdocs.com/display/parserjava/Parse+data+from+PDF+documents)

निम्न उदाहरण दर्शाता है कि दस्तावेज़ के फ़ॉर्म को कैसे पार्स किया जाए:

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


दस्तावेज़ से संरचित पाठ निकालता है।

**Learn more:**

* [Extract text structure](../https://docs.groupdocs.com/display/parserjava/Extract+text+structure)


**Returns:**
org.w3c.dom.Document - XML टेक्स्ट संरचना वाले org.w3c.dom.Document क्लास का एक इंस्टेंस; यदि टेक्स्ट संरचना निष्कर्षण समर्थित नहीं है तो null।

### close() {#close--}
```
public void close()
```


इस संसाधन को बंद करता है, सभी अंतर्निहित संसाधनों को मुक्त करता है।


