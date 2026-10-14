---
title: "LoadOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per aprire un file."
type: docs
weight: 24
url: /it/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Fornisce le opzioni utilizzate per aprire un file.

Un'istanza di questa classe è usata come parametro nei costruttori della classe [Parser](../../com.groupdocs.parser/parser):

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Vedi gli esempi di utilizzo lì.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con timeout. |
|
|  | [LoadOptions()](#LoadOptions--) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vuota, FileFormat uguale a FileFormat.Unknown e codifiche predefinite. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con FileFormat uguale a FileFormat.Unknown e codifiche predefinite. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vuota e codifiche predefinite. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codifiche predefinite. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codifiche personalizzate. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) completamente personalizzata. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vuota e codifiche predefinite. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con password e codifiche predefinite. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codifiche personalizzate. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) completamente personalizzata. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Restituisce il formato del file. |
|
|  | [getFileType()](#getFileType--) | Restituisce il tipo di file. |
|
|  | [getPassword()](#getPassword--) | Ottiene la password. |
|
|  | [getCharset()](#getCharset--) | Restituisce la codifica del documento. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Restituisce la codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
|
|  | [getTimeout()](#getTimeout--) | Restituisce il valore che rappresenta il numero di millisecondi da attendere. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con timeout.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | tempo di attesa | java.time.Duration | La Duration che rappresenta il numero di millisecondi da attendere. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vuota, FileFormat uguale a FileFormat.Unknown e codifiche predefinite.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con FileFormat uguale a FileFormat.Unknown e codifiche predefinite.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vuota e codifiche predefinite.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Il formato del file. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codifiche predefinite.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Il formato del file. |
|
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codifiche personalizzate.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Il formato del file. |
|
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|
|  | charset | java.nio.charset.Charset | La codifica del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) completamente personalizzata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Il formato del file. |
|
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|
|  | charset | java.nio.charset.Charset | La codifica del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
|
|  | tempo di attesa | java.time.Duration | La Duration che rappresenta il numero di millisecondi da attendere. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vuota e codifiche predefinite.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Il tipo del file. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con password e codifiche predefinite.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Il tipo del file. |
|
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codifiche personalizzate.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Il tipo del file. |
|
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|
|  | charset | java.nio.charset.Charset | La codifica del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Inizializza una nuova istanza della classe [LoadOptions](../../com.groupdocs.parser.options/loadoptions) completamente personalizzata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Il tipo del file. |
|
|  | password | java.lang.String | La password per aprire il file protetto da password. |
|
|  | charset | java.nio.charset.Charset | La codifica del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codifica ANSI predefinita utilizzata per il rilevamento della codifica. |
|
|  | tempo di attesa | java.time.Duration | La Duration che rappresenta il numero di millisecondi da attendere. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Restituisce il formato del file.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Restituisce il tipo di file.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Ottiene la password.


**Returns:**
java.lang.String - Un valore stringa che rappresenta una password per aprire il file protetto da password.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Restituisce la codifica del documento.


**Returns:**
java.nio.charset.Charset - Un'istanza della classe Charset che rappresenta la codifica del documento; null se non è impostata.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Restituisce la codifica ANSI predefinita utilizzata per il rilevamento della codifica.


**Returns:**
java.nio.charset.Charset - Un'istanza della classe Charset che rappresenta la codifica del documento; null se non è impostata.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Restituisce il valore che rappresenta il numero di millisecondi da attendere.


**Returns:**
java.time.Duration - Un'istanza di Duration che rappresenta il numero di millisecondi da attendere.

