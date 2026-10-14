---
title: "FileFormat"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يحدد نوع الملف."
type: docs
weight: 43
url: /ar/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

يحدد نوع الملف.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Unknown](#Unknown) | القيمة الافتراضية. |
|
|  | [WordProcessing](#WordProcessing) | مستند معالجة نصوص (DOC, DOCX, ODT, إلخ). |
|
|  | [Spreadsheet](#Spreadsheet) | مستند جدول بيانات (XLS, XLSX, ODS, إلخ). |
|
|  | [Presentation](#Presentation) | مستند عرض تقديمي (PPT, PPTX, ODP, إلخ). |
|
|  | [Email](#Email) | مستند بريد إلكتروني (رسائل البريد الإلكتروني أو حاويات رسائل البريد الإلكتروني). |
|
|  | [Pdf](#Pdf) | مستند PDF. |
|
|  | [Markup](#Markup) | مستند توصيف (HTML, XML, Markdown, إلخ). |
|
|  | [Ebook](#Ebook) | مستند كتاب إلكتروني (ePUB, FictionBook, إلخ). |
|
|  | [Note](#Note) | مستند ملاحظة. |
|
|  | [Archive](#Archive) | ملف أرشيف. |
|
|  | [Database](#Database) | ملفات قاعدة البيانات (عبر JDBC). |
|
|  | [Image](#Image) | ملف صورة. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


القيمة الافتراضية.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


مستند معالجة نصوص (DOC, DOCX, ODT, إلخ).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


مستند جدول بيانات (XLS, XLSX, ODS, إلخ).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


مستند عرض تقديمي (PPT, PPTX, ODP, إلخ).


### Email {#Email}
```
public static final FileFormat Email
```


مستند بريد إلكتروني (رسائل البريد الإلكتروني أو حاويات رسائل البريد الإلكتروني).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


مستند PDF.


### Markup {#Markup}
```
public static final FileFormat Markup
```


مستند توصيف (HTML, XML, Markdown, إلخ).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


مستند كتاب إلكتروني (ePUB, FictionBook, إلخ).


### Note {#Note}
```
public static final FileFormat Note
```


مستند ملاحظة.


### Archive {#Archive}
```
public static final FileFormat Archive
```


ملف أرشيف.


### Database {#Database}
```
public static final FileFormat Database
```


ملفات قاعدة البيانات (عبر JDBC).


### Image {#Image}
```
public static final FileFormat Image
```


ملف صورة.


### values() {#values--}
```
public static FileFormat[] values()
```




**Returns:**
com.groupdocs.parser.options.FileFormat[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileFormat valueOf(String name)
```




**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
