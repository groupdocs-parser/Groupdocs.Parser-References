---
title: "FileFormat"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Define un tipo de archivo."
type: docs
weight: 43
url: /es/java/com.groupdocs.parser.options/fileformat/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileFormat extends Enum<FileFormat>
```

Define un tipo de archivo.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Unknown](#Unknown) | Valor predeterminado. |
|
|  | [WordProcessing](#WordProcessing) | Documento de procesamiento de texto (DOC, DOCX, ODT, etc). |
|
|  | [Spreadsheet](#Spreadsheet) | Documento de hoja de cálculo (XLS, XLSX, ODS, etc). |
|
|  | [Presentation](#Presentation) | Documento de presentación (PPT, PPTX, ODP, etc). |
|
|  | [Email](#Email) | Documento de correo electrónico (mensajes de correo o contenedores de mensajes de correo). |
|
|  | [Pdf](#Pdf) | Documento PDF. |
|
|  | [Markup](#Markup) | Documento de marcado (HTML, XML, Markdown, etc). |
|
|  | [Ebook](#Ebook) | Documento de libro electrónico (ePUB, FictionBook, etc). |
|
|  | [Note](#Note) | Documento de notas. |
|
|  | [Archive](#Archive) | Archivo de archivo. |
|
|  | [Database](#Database) | Archivos de base de datos (a través de JDBC). |
|
|  | [Image](#Image) | Archivo de imagen. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Unknown {#Unknown}
```
public static final FileFormat Unknown
```


Valor predeterminado.


### WordProcessing {#WordProcessing}
```
public static final FileFormat WordProcessing
```


Documento de procesamiento de texto (DOC, DOCX, ODT, etc).


### Spreadsheet {#Spreadsheet}
```
public static final FileFormat Spreadsheet
```


Documento de hoja de cálculo (XLS, XLSX, ODS, etc).


### Presentation {#Presentation}
```
public static final FileFormat Presentation
```


Documento de presentación (PPT, PPTX, ODP, etc).


### Email {#Email}
```
public static final FileFormat Email
```


Documento de correo electrónico (mensajes de correo o contenedores de mensajes de correo).


### Pdf {#Pdf}
```
public static final FileFormat Pdf
```


Documento PDF.


### Markup {#Markup}
```
public static final FileFormat Markup
```


Documento de marcado (HTML, XML, Markdown, etc).


### Ebook {#Ebook}
```
public static final FileFormat Ebook
```


Documento de libro electrónico (ePUB, FictionBook, etc).


### Note {#Note}
```
public static final FileFormat Note
```


Documento de notas.


### Archive {#Archive}
```
public static final FileFormat Archive
```


Archivo de archivo.


### Database {#Database}
```
public static final FileFormat Database
```


Archivos de base de datos (a través de JDBC).


### Image {#Image}
```
public static final FileFormat Image
```


Archivo de imagen.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat)
