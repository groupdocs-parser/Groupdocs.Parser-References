---
title: "FileFormat"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Definiert einen Dateityp."
type: docs
weight: 43
url: /de/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

Definiert einen Dateityp.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Unknown](#Unknown) | Standardwert. |
|
|  | [WordProcessing](#WordProcessing) | Textverarbeitungsdokument (DOC, DOCX, ODT usw.). |
|
|  | [Spreadsheet](#Spreadsheet) | Tabellendokument (XLS, XLSX, ODS usw.). |
|
|  | [Presentation](#Presentation) | Präsentationsdokument (PPT, PPTX, ODP usw.). |
|
|  | [Email](#Email) | E‑Mail‑Dokument (E‑Mail‑Nachrichten oder E‑Mail‑Nachrichtcontainer). |
|
|  | [Pdf](#Pdf) | PDF‑Dokument. |
|
|  | [Markup](#Markup) | Markup‑Dokument (HTML, XML, Markdown usw.). |
|
|  | [Ebook](#Ebook) | E‑Book‑Dokument (ePUB, FictionBook usw.). |
|
|  | [Note](#Note) | Notiz‑Dokument. |
|
|  | [Archive](#Archive) | Archivdatei. |
|
|  | [Database](#Database) | Datenbankdateien (via JDBC). |
|
|  | [Image](#Image) | Bilddatei. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


Standardwert.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


Textverarbeitungsdokument (DOC, DOCX, ODT usw.).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


Tabellendokument (XLS, XLSX, ODS usw.).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


Präsentationsdokument (PPT, PPTX, ODP usw.).


### Email {#Email}
```
public static final FileFormat Email
```


E‑Mail‑Dokument (E‑Mail‑Nachrichten oder E‑Mail‑Nachrichtcontainer).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


PDF‑Dokument.


### Markup {#Markup}
```
public static final FileFormat Markup
```


Markup‑Dokument (HTML, XML, Markdown usw.).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


E‑Book‑Dokument (ePUB, FictionBook usw.).


### Note {#Note}
```
public static final FileFormat Note
```


Notiz‑Dokument.


### Archive {#Archive}
```
public static final FileFormat Archive
```


Archivdatei.


### Database {#Database}
```
public static final FileFormat Database
```


Datenbankdateien (via JDBC).


### Image {#Image}
```
public static final FileFormat Image
```


Bilddatei.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
