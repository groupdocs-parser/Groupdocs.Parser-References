---
title: "FileFormat"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "파일 유형을 정의합니다."
type: docs
weight: 43
url: /ko/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

파일 유형을 정의합니다.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Unknown](#Unknown) | 기본값. |
|
|  | [WordProcessing](#WordProcessing) | 워드 프로세싱 문서 (DOC, DOCX, ODT 등). |
|
|  | [Spreadsheet](#Spreadsheet) | 스프레드시트 문서 (XLS, XLSX, ODS 등). |
|
|  | [Presentation](#Presentation) | 프레젠테이션 문서 (PPT, PPTX, ODP 등). |
|
|  | [Email](#Email) | 이메일 문서 (이메일 메시지 또는 이메일 메시지 컨테이너). |
|
|  | [Pdf](#Pdf) | PDF 문서. |
|
|  | [Markup](#Markup) | 마크업 문서 (HTML, XML, Markdown 등). |
|
|  | [Ebook](#Ebook) | 전자책 문서 (ePUB, FictionBook 등). |
|
|  | [Note](#Note) | 노트 문서. |
|
|  | [Archive](#Archive) | 아카이브 파일. |
|
|  | [Database](#Database) | 데이터베이스 파일 (JDBC를 통해). |
|
|  | [Image](#Image) | 이미지 파일. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


기본값.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


워드 프로세싱 문서 (DOC, DOCX, ODT 등).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


스프레드시트 문서 (XLS, XLSX, ODS 등).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


프레젠테이션 문서 (PPT, PPTX, ODP 등).


### Email {#Email}
```
public static final FileFormat Email
```


이메일 문서 (이메일 메시지 또는 이메일 메시지 컨테이너).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


PDF 문서.


### Markup {#Markup}
```
public static final FileFormat Markup
```


마크업 문서 (HTML, XML, Markdown 등).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


전자책 문서 (ePUB, FictionBook 등).


### Note {#Note}
```
public static final FileFormat Note
```


노트 문서.


### Archive {#Archive}
```
public static final FileFormat Archive
```


아카이브 파일.


### Database {#Database}
```
public static final FileFormat Database
```


데이터베이스 파일 (JDBC를 통해).


### Image {#Image}
```
public static final FileFormat Image
```


이미지 파일.


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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
