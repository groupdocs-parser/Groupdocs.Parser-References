---
title: "FileFormat"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Définit un type de fichier."
type: docs
weight: 43
url: /fr/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

Définit un type de fichier.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## Champs

| Champ | Description |
| --- | --- |
|  | [Unknown](#Unknown) | Valeur par défaut. |
|
|  | [WordProcessing](#WordProcessing) | Document de traitement de texte (DOC, DOCX, ODT, etc). |
|
|  | [Spreadsheet](#Spreadsheet) | Document de feuille de calcul (XLS, XLSX, ODS, etc). |
|
|  | [Presentation](#Presentation) | Document de présentation (PPT, PPTX, ODP, etc). |
|
|  | [Email](#Email) | Document de messagerie (messages électroniques ou conteneurs de messages électroniques). |
|
|  | [Pdf](#Pdf) | Document PDF. |
|
|  | [Markup](#Markup) | Document de balisage (HTML, XML, Markdown, etc). |
|
|  | [Ebook](#Ebook) | Document ebook (ePUB, FictionBook, etc). |
|
|  | [Note](#Note) | Document de note. |
|
|  | [Archive](#Archive) | Fichier d'archive. |
|
|  | [Database](#Database) | Fichiers de base de données (via JDBC). |
|
|  | [Image](#Image) | Fichier image. |
|
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


Valeur par défaut.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


Document de traitement de texte (DOC, DOCX, ODT, etc).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


Document de feuille de calcul (XLS, XLSX, ODS, etc).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


Document de présentation (PPT, PPTX, ODP, etc).


### Email {#Email}
```
public static final FileFormat Email
```


Document de messagerie (messages électroniques ou conteneurs de messages électroniques).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


Document PDF.


### Markup {#Markup}
```
public static final FileFormat Markup
```


Document de balisage (HTML, XML, Markdown, etc).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


Document ebook (ePUB, FictionBook, etc).


### Note {#Note}
```
public static final FileFormat Note
```


Document de note.


### Archive {#Archive}
```
public static final FileFormat Archive
```


Fichier d'archive.


### Database {#Database}
```
public static final FileFormat Database
```


Fichiers de base de données (via JDBC).


### Image {#Image}
```
public static final FileFormat Image
```


Fichier image.


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
| Parameter | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
