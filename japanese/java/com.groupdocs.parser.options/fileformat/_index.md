---
title: "FileFormat"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ファイルのタイプを定義します。"
type: docs
weight: 43
url: /ja/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

ファイルのタイプを定義します。

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Unknown](#Unknown) | 既定値です。 |
|
|  | [WordProcessing](#WordProcessing) | ワードプロセッシング文書（DOC、DOCX、ODT など）。 |
|
|  | [Spreadsheet](#Spreadsheet) | スプレッドシート文書（XLS、XLSX、ODS など）。 |
|
|  | [Presentation](#Presentation) | プレゼンテーション文書（PPT、PPTX、ODP など）。 |
|
|  | [Email](#Email) | メール文書（メールメッセージまたはメールメッセージコンテナ）。 |
|
|  | [Pdf](#Pdf) | PDF 文書です。 |
|
|  | [Markup](#Markup) | マークアップ文書（HTML、XML、Markdown など）。 |
|
|  | [Ebook](#Ebook) | 電子書籍文書（ePUB、FictionBook など）。 |
|
|  | [Note](#Note) | ノート文書です。 |
|
|  | [Archive](#Archive) | アーカイブ ファイルです。 |
|
|  | [Database](#Database) | データベースファイル（JDBC 経由）。 |
|
|  | [Image](#Image) | 画像ファイルです。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


既定値です。


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


ワードプロセッシング文書（DOC、DOCX、ODT など）。


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


スプレッドシート文書（XLS、XLSX、ODS など）。


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


プレゼンテーション文書（PPT、PPTX、ODP など）。


### Email {#Email}
```
public static final FileFormat Email
```


メール文書（メールメッセージまたはメールメッセージコンテナ）。


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


PDF 文書です。


### Markup {#Markup}
```
public static final FileFormat Markup
```


マークアップ文書（HTML、XML、Markdown など）。


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


電子書籍文書（ePUB、FictionBook など）。


### Note {#Note}
```
public static final FileFormat Note
```


ノート文書です。


### Archive {#Archive}
```
public static final FileFormat Archive
```


アーカイブ ファイルです。


### Database {#Database}
```
public static final FileFormat Database
```


データベースファイル（JDBC 経由）。


### Image {#Image}
```
public static final FileFormat Image
```


画像ファイルです。


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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
