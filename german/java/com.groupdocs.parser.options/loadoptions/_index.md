---
title: "LoadOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die zum Öffnen einer Datei verwendet werden."
type: docs
weight: 24
url: /de/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Stellt die Optionen bereit, die zum Öffnen einer Datei verwendet werden.

Eine Instanz dieser Klasse wird als Parameter in den Konstruktoren der Klasse [Parser](../../com.groupdocs.parser/parser) verwendet:

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit timeout. |
|
|  | [LoadOptions()](#LoadOptions--) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit leerem Password, FileFormat gleich FileFormat.Unknown und Standardkodierungen. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit FileFormat gleich FileFormat.Unknown und Standardkodierungen. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit leerem Password und Standardkodierungen. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit Standardkodierungen. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit benutzerdefinierten Kodierungen. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initialisiert eine neue Instanz der vollständig angepassten Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit leerem Password und Standardkodierungen. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Initialisiert eine neue Instanz der [LoadOptions](../../com.groupdocs.parser.options/loadoptions)-Klasse mit Passwort und Standardkodierungen. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit benutzerdefinierten Kodierungen. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initialisiert eine neue Instanz der vollständig angepassten Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Ermittelt das Dateiformat. |
|
|  | [getFileType()](#getFileType--) | Ermittelt den Dateityp. |
|
|  | [getPassword()](#getPassword--) | Liefert das Passwort. |
|
|  | [getCharset()](#getCharset--) | Ermittelt die Kodierung des Dokuments. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Ermittelt die standardmäßige ANSI‑Kodierung, die zur Kodierungserkennung verwendet wird. |
|
|  | [getTimeout()](#getTimeout--) | Ermittelt den Wert, der die Anzahl der Millisekunden zum Warten darstellt. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit timeout.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Timeout | java.time.Duration | Die Duration, die die Anzahl der Millisekunden zum Warten darstellt. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit leerem Password, FileFormat gleich FileFormat.Unknown und Standardkodierungen.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit FileFormat gleich FileFormat.Unknown und Standardkodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit leerem Password und Standardkodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Das Format der Datei. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit Standardkodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Das Format der Datei. |
|
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit benutzerdefinierten Kodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Das Format der Datei. |
|
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|
|  | charset | java.nio.charset.Charset | Die Kodierung des Dokuments. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Die standardmäßige ANSI‑Kodierung, die zur Kodierungserkennung verwendet wird. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initialisiert eine neue Instanz der vollständig angepassten Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Das Format der Datei. |
|
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|
|  | charset | java.nio.charset.Charset | Die Kodierung des Dokuments. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Die standardmäßige ANSI‑Kodierung, die zur Kodierungserkennung verwendet wird. |
|
|  | Timeout | java.time.Duration | Die Duration, die die Anzahl der Millisekunden zum Warten darstellt. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit leerem Password und Standardkodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Der Typ der Datei. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Initialisiert eine neue Instanz der [LoadOptions](../../com.groupdocs.parser.options/loadoptions)-Klasse mit Passwort und Standardkodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Der Typ der Datei. |
|
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Initialisiert eine neue Instanz der Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions) mit benutzerdefinierten Kodierungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Der Typ der Datei. |
|
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|
|  | charset | java.nio.charset.Charset | Die Kodierung des Dokuments. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Die standardmäßige ANSI‑Kodierung, die zur Kodierungserkennung verwendet wird. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initialisiert eine neue Instanz der vollständig angepassten Klasse [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Der Typ der Datei. |
|
|  | Passwort | java.lang.String | Das Passwort, um die passwortgeschützte Datei zu öffnen. |
|
|  | charset | java.nio.charset.Charset | Die Kodierung des Dokuments. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Die standardmäßige ANSI‑Kodierung, die zur Kodierungserkennung verwendet wird. |
|
|  | Timeout | java.time.Duration | Die Duration, die die Anzahl der Millisekunden zum Warten darstellt. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Ermittelt das Dateiformat.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Ermittelt den Dateityp.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Liefert das Passwort.


**Returns:**
java.lang.String – Ein String‑Wert, der ein Passwort zum Öffnen der passwortgeschützten Datei darstellt.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Ermittelt die Kodierung des Dokuments.


**Returns:**
java.nio.charset.Charset – Eine Instanz der  Charset ‑Klasse, die die Dokumentenkodierung darstellt;  null  falls sie nicht gesetzt ist.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Ermittelt die standardmäßige ANSI‑Kodierung, die zur Kodierungserkennung verwendet wird.


**Returns:**
java.nio.charset.Charset – Eine Instanz der  Charset ‑Klasse, die die Dokumentenkodierung darstellt;  null  falls sie nicht gesetzt ist.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Ermittelt den Wert, der die Anzahl der Millisekunden zum Warten darstellt.


**Returns:**
java.time.Duration – Eine Instanz von Duration, die die Anzahl der Millisekunden zum Warten darstellt.

