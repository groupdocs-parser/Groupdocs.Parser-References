---
title: "LoadOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Bir dosya açmak için kullanılan seçenekleri sağlar."
type: docs
weight: 24
url: /tr/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Bir dosya açmak için kullanılan seçenekleri sağlar.

Bu sınıfın bir örneği, [Parser](../../com.groupdocs.parser/parser) sınıfı yapıcılarında parametre olarak kullanılır:

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Oradaki kullanım örneklerine bakın.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini timeout ile başlatır. |
|
|  | [LoadOptions()](#LoadOptions--) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini boş  Password ,  FileFormat  eşit FileFormat.Unknown  ve varsayılan kodlamalar ile başlatır. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini  FileFormat  eşit FileFormat.Unknown  ve varsayılan kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini boş  Password  ve varsayılan kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini varsayılan kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini özel kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfını tamamen özelleştirilmiş şekilde başlatır. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini boş  Password  ve varsayılan kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini password ve varsayılan kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini özel kodlamalar ile başlatır. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfını tamamen özelleştirilmiş şekilde başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Dosya formatını alır. |
|
|  | [getFileType()](#getFileType--) | Dosya türünü alır. |
|
|  | [getPassword()](#getPassword--) | Parolayı alır. |
|
|  | [getCharset()](#getCharset--) | Belgenin kodlamasını alır. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Kodlama tespiti için kullanılan varsayılan ANSI kodlamasını alır. |
|
|  | [getTimeout()](#getTimeout--) | Bekleme süresi milisaniye sayısını temsil eden değeri alır. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini timeout ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | timeout | java.time.Duration | Bekleme süresi milisaniye sayısını temsil eden Duration. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini boş  Password ,  FileFormat  eşit FileFormat.Unknown  ve varsayılan kodlamalar ile başlatır.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini  FileFormat  eşit FileFormat.Unknown  ve varsayılan kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini boş  Password  ve varsayılan kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Dosyanın formatı. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini varsayılan kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Dosyanın formatı. |
|
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini özel kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Dosyanın formatı. |
|
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|
|  | charset | java.nio.charset.Charset | Belgenin kodlaması. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Kodlama tespiti için kullanılan varsayılan ANSI kodlaması. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfını tamamen özelleştirilmiş şekilde başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Dosyanın formatı. |
|
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|
|  | charset | java.nio.charset.Charset | Belgenin kodlaması. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Kodlama tespiti için kullanılan varsayılan ANSI kodlaması. |
|
|  | timeout | java.time.Duration | Bekleme süresi milisaniye sayısını temsil eden Duration. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini boş  Password  ve varsayılan kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Dosyanın türü. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini password ve varsayılan kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Dosyanın türü. |
|
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfı örneğini özel kodlamalar ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Dosyanın türü. |
|
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|
|  | charset | java.nio.charset.Charset | Belgenin kodlaması. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Kodlama tespiti için kullanılan varsayılan ANSI kodlaması. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Yeni bir [LoadOptions](../../com.groupdocs.parser.options/loadoptions) sınıfını tamamen özelleştirilmiş şekilde başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Dosyanın türü. |
|
|  | parola | java.lang.String | Parola korumalı dosyayı açmak için password. |
|
|  | charset | java.nio.charset.Charset | Belgenin kodlaması. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Kodlama tespiti için kullanılan varsayılan ANSI kodlaması. |
|
|  | timeout | java.time.Duration | Bekleme süresi milisaniye sayısını temsil eden Duration. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Dosya formatını alır.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Dosya türünü alır.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Parolayı alır.


**Returns:**
java.lang.String - Parola korumalı dosyayı açmak için bir şifreyi temsil eden dize değeri.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Belgenin kodlamasını alır.


**Returns:**
java.nio.charset.Charset - Belge kodlamasını temsil eden Charset sınıfının bir örneği; ayarlanmamışsa null.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Kodlama tespiti için kullanılan varsayılan ANSI kodlamasını alır.


**Returns:**
java.nio.charset.Charset - Belge kodlamasını temsil eden Charset sınıfının bir örneği; ayarlanmamışsa null.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Bekleme süresi milisaniye sayısını temsil eden değeri alır.


**Returns:**
java.time.Duration - Bekleme süresini milisaniye cinsinden temsil eden Duration sınıfının bir örneği.

