---
title: "LoadOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt om een bestand te openen."
type: docs
weight: 24
url: /nl/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Biedt de opties die worden gebruikt om een bestand te openen.

Een exemplaar van deze klasse wordt gebruikt als parameter in de constructors van de [Parser](../../com.groupdocs.parser/parser) klasse:

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Zie daar de gebruiksvoorbeelden.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met  timeout . |
|
|  | [LoadOptions()](#LoadOptions--) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met een lege  Password ,  FileFormat  gelijk aan  FileFormat.Unknown  en standaardcoderingen. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met  FileFormat  gelijk aan  FileFormat.Unknown  en standaardcoderingen. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met een lege  Password  en standaardcoderingen. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met standaardcoderingen. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met aangepaste coderingen. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initialiseert een nieuw exemplaar van de volledig aangepaste [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met een lege  Password  en standaardcoderingen. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met wachtwoord en standaardcoderingen. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met aangepaste coderingen. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initialiseert een nieuw exemplaar van de volledig aangepaste [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Haalt het bestandsformaat op. |
|
|  | [getFileType()](#getFileType--) | Haalt het bestandstype op. |
|
|  | [getPassword()](#getPassword--) | Haalt het wachtwoord op. |
|
|  | [getCharset()](#getCharset--) | Haalt de codering van het document op. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Haalt de standaard ANSI-codering op die wordt gebruikt voor coderingsdetectie. |
|
|  | [getTimeout()](#getTimeout--) | Haalt de waarde op die het aantal milliseconden om te wachten vertegenwoordigt. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met  timeout .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | timeout | java.time.Duration | De Duration die het aantal milliseconden om te wachten vertegenwoordigt. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met een lege  Password ,  FileFormat  gelijk aan  FileFormat.Unknown  en standaardcoderingen.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met  FileFormat  gelijk aan  FileFormat.Unknown  en standaardcoderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met een lege  Password  en standaardcoderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Het formaat van het bestand. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met standaardcoderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Het formaat van het bestand. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met aangepaste coderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Het formaat van het bestand. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|
|  | charset | java.nio.charset.Charset | De codering van het document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | De standaard ANSI-codering die wordt gebruikt voor coderingsdetectie. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initialiseert een nieuw exemplaar van de volledig aangepaste [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Het formaat van het bestand. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|
|  | charset | java.nio.charset.Charset | De codering van het document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | De standaard ANSI-codering die wordt gebruikt voor coderingsdetectie. |
|
|  | timeout | java.time.Duration | De Duration die het aantal milliseconden om te wachten vertegenwoordigt. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met een lege  Password  en standaardcoderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Het type van het bestand. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met wachtwoord en standaardcoderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Het type van het bestand. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Initialiseert een nieuw exemplaar van de [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse met aangepaste coderingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Het type van het bestand. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|
|  | charset | java.nio.charset.Charset | De codering van het document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | De standaard ANSI-codering die wordt gebruikt voor coderingsdetectie. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initialiseert een nieuw exemplaar van de volledig aangepaste [LoadOptions](../../com.groupdocs.parser.options/loadoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Het type van het bestand. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord om het met wachtwoord beveiligde bestand te openen. |
|
|  | charset | java.nio.charset.Charset | De codering van het document. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | De standaard ANSI-codering die wordt gebruikt voor coderingsdetectie. |
|
|  | timeout | java.time.Duration | De Duration die het aantal milliseconden om te wachten vertegenwoordigt. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Haalt het bestandsformaat op.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Haalt het bestandstype op.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Haalt het wachtwoord op.


**Returns:**
java.lang.String - Een stringwaarde die een wachtwoord vertegenwoordigt om het met wachtwoord beveiligde bestand te openen.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Haalt de codering van het document op.


**Returns:**
java.nio.charset.Charset - Een instantie van de  Charset  klasse die de documentcodering vertegenwoordigt;  null  als deze niet is ingesteld.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Haalt de standaard ANSI-codering op die wordt gebruikt voor coderingsdetectie.


**Returns:**
java.nio.charset.Charset - Een instantie van de  Charset  klasse die de documentcodering vertegenwoordigt;  null  als deze niet is ingesteld.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Haalt de waarde op die het aantal milliseconden om te wachten vertegenwoordigt.


**Returns:**
java.time.Duration - Een instantie van Duration die het aantal milliseconden om te wachten vertegenwoordigt.

