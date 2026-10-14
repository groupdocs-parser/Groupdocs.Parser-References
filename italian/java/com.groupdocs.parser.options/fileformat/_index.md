---
title: "FileFormat"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Definisce un tipo di file."
type: docs
weight: 43
url: /it/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

Definisce un tipo di file.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Unknown](#Unknown) | Valore predefinito. |
|
|  | [WordProcessing](#WordProcessing) | Documento di elaborazione testi (DOC, DOCX, ODT, ecc). |
|
|  | [Spreadsheet](#Spreadsheet) | Documento di foglio di calcolo (XLS, XLSX, ODS, ecc). |
|
|  | [Presentation](#Presentation) | Documento di presentazione (PPT, PPTX, ODP, ecc). |
|
|  | [Email](#Email) | Documento email (messaggi email o contenitori di messaggi email). |
|
|  | [Pdf](#Pdf) | Documento PDF. |
|
|  | [Markup](#Markup) | Documento di markup (HTML, XML, Markdown, ecc). |
|
|  | [Ebook](#Ebook) | Documento ebook (ePUB, FictionBook, ecc). |
|
|  | [Note](#Note) | Documento di note. |
|
|  | [Archive](#Archive) | File di archivio. |
|
|  | [Database](#Database) | File di database (tramite JDBC). |
|
|  | [Image](#Image) | File immagine. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


Valore predefinito.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


Documento di elaborazione testi (DOC, DOCX, ODT, ecc).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


Documento di foglio di calcolo (XLS, XLSX, ODS, ecc).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


Documento di presentazione (PPT, PPTX, ODP, ecc).


### Email {#Email}
```
public static final FileFormat Email
```


Documento email (messaggi email o contenitori di messaggi email).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


Documento PDF.


### Markup {#Markup}
```
public static final FileFormat Markup
```


Documento di markup (HTML, XML, Markdown, ecc).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


Documento ebook (ePUB, FictionBook, ecc).


### Note {#Note}
```
public static final FileFormat Note
```


Documento di note.


### Archive {#Archive}
```
public static final FileFormat Archive
```


File di archivio.


### Database {#Database}
```
public static final FileFormat Database
```


File di database (tramite JDBC).


### Image {#Image}
```
public static final FileFormat Image
```


File immagine.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
