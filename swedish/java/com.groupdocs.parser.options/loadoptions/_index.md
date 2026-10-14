---
title: "LoadOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för att öppna en fil."
type: docs
weight: 24
url: /sv/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Tillhandahåller de alternativ som används för att öppna en fil.

En instans av den här klassen används som parameter i konstruktörer för klassen [Parser](../../com.groupdocs.parser/parser):

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Se användningsexemplen där.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med timeout. |
|
|  | [LoadOptions()](#LoadOptions--) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med tomt Password, FileFormat lika med FileFormat.Unknown och standardkodningar. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med FileFormat lika med FileFormat.Unknown och standardkodningar. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med tomt Password och standardkodningar. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med standardkodningar. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med anpassade kodningar. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initierar en ny instans av den fullt anpassade klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med tomt Password och standardkodningar. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med lösenord och standardkodningar. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med anpassade kodningar. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Initierar en ny instans av den fullt anpassade klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Hämtar filformatet. |
|
|  | [getFileType()](#getFileType--) | Hämtar filtypen. |
|
|  | [getPassword()](#getPassword--) | Hämtar lösenordet. |
|
|  | [getCharset()](#getCharset--) | Hämtar kodningen för dokumentet. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Hämtar standard-ANSI-kodning som används för kodningsdetektering. |
|
|  | [getTimeout()](#getTimeout--) | Hämtar värdet som representerar antalet millisekunder att vänta. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med timeout.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | timeout | java.time.Duration | Duration-objektet som representerar antalet millisekunder att vänta. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med tomt Password, FileFormat lika med FileFormat.Unknown och standardkodningar.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med FileFormat lika med FileFormat.Unknown och standardkodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med tomt Password och standardkodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Formatet för filen. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med standardkodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Formatet för filen. |
|
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med anpassade kodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Formatet för filen. |
|
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|
|  | charset | java.nio.charset.Charset | Kodningen för dokumentet. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Standard-ANSI-kodning som används för kodningsdetektering. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initierar en ny instans av den fullt anpassade klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Formatet för filen. |
|
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|
|  | charset | java.nio.charset.Charset | Kodningen för dokumentet. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Standard-ANSI-kodning som används för kodningsdetektering. |
|
|  | timeout | java.time.Duration | Duration-objektet som representerar antalet millisekunder att vänta. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med tomt Password och standardkodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Typen av filen. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med lösenord och standardkodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Typen av filen. |
|
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Initierar en ny instans av klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions) med anpassade kodningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Typen av filen. |
|
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|
|  | charset | java.nio.charset.Charset | Kodningen för dokumentet. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Standard-ANSI-kodning som används för kodningsdetektering. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Initierar en ny instans av den fullt anpassade klassen [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Typen av filen. |
|
|  | lösenord | java.lang.String | Lösenordet för att öppna den lösenordsskyddade filen. |
|
|  | charset | java.nio.charset.Charset | Kodningen för dokumentet. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Standard-ANSI-kodning som används för kodningsdetektering. |
|
|  | timeout | java.time.Duration | Duration-objektet som representerar antalet millisekunder att vänta. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Hämtar filformatet.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Hämtar filtypen.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Hämtar lösenordet.


**Returns:**
java.lang.String – Ett strängvärde som representerar ett lösenord för att öppna den lösenordsskyddade filen.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Hämtar kodningen för dokumentet.


**Returns:**
java.nio.charset.Charset – En instans av klassen Charset som representerar dokumentets kodning; null om den inte är angiven.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Hämtar standard-ANSI-kodning som används för kodningsdetektering.


**Returns:**
java.nio.charset.Charset – En instans av klassen Charset som representerar dokumentets kodning; null om den inte är angiven.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Hämtar värdet som representerar antalet millisekunder att vänta.


**Returns:**
java.time.Duration – En instans av Duration som representerar antalet millisekunder att vänta.

