---
title: "FileFormat"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Определяет тип файла."
type: docs
weight: 43
url: /ru/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

Определяет тип файла.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## Поля

| Поле | Описание |
| --- | --- |
|  | [Unknown](#Unknown) | Значение по умолчанию. |
|
|  | [WordProcessing](#WordProcessing) | Документ обработки текста (DOC, DOCX, ODT и т.д.). |
|
|  | [Spreadsheet](#Spreadsheet) | Электронная таблица (XLS, XLSX, ODS и т.д.). |
|
|  | [Presentation](#Presentation) | Презентация (PPT, PPTX, ODP и т.д.). |
|
|  | [Email](#Email) | Электронное письмо (сообщения электронной почты или контейнеры сообщений). |
|
|  | [Pdf](#Pdf) | PDF‑документ. |
|
|  | [Markup](#Markup) | Разметочный документ (HTML, XML, Markdown и т.д.). |
|
|  | [Ebook](#Ebook) | Электронная книга (ePUB, FictionBook и т.д.). |
|
|  | [Note](#Note) | Заметка. |
|
|  | [Archive](#Archive) | Архивный файл. |
|
|  | [Database](#Database) | Файлы базы данных (через JDBC). |
|
|  | [Image](#Image) | Файл изображения. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


Значение по умолчанию.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


Документ обработки текста (DOC, DOCX, ODT и т.д.).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


Электронная таблица (XLS, XLSX, ODS и т.д.).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


Презентация (PPT, PPTX, ODP и т.д.).


### Email {#Email}
```
public static final FileFormat Email
```


Электронное письмо (сообщения электронной почты или контейнеры сообщений).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


PDF‑документ.


### Markup {#Markup}
```
public static final FileFormat Markup
```


Разметочный документ (HTML, XML, Markdown и т.д.).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


Электронная книга (ePUB, FictionBook и т.д.).


### Note {#Note}
```
public static final FileFormat Note
```


Заметка.


### Archive {#Archive}
```
public static final FileFormat Archive
```


Архивный файл.


### Database {#Database}
```
public static final FileFormat Database
```


Файлы базы данных (через JDBC).


### Image {#Image}
```
public static final FileFormat Image
```


Файл изображения.


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
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
