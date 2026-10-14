---
title: "LoadOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk membuka file."
type: docs
weight: 24
url: /id/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Menyediakan opsi yang digunakan untuk membuka file.

Sebuah instance dari kelas ini digunakan sebagai parameter dalam konstruktor kelas [Parser](../../com.groupdocs.parser/parser):

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Lihat contoh penggunaan di sana.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan timeout . |
|
|  | [LoadOptions()](#LoadOptions--) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan Password kosong, FileFormat sama dengan FileFormat.Unknown, dan enkoding default. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan FileFormat sama dengan FileFormat.Unknown dan enkoding default. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan Password kosong dan enkoding default. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan enkoding default. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan enkoding khusus. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) yang sepenuhnya disesuaikan. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan Password kosong dan enkoding default. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan kata sandi dan enkoding default. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan enkoding khusus. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) yang sepenuhnya disesuaikan. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Mendapatkan format file. |
|
|  | [getFileType()](#getFileType--) | Mendapatkan tipe file. |
|
|  | [getPassword()](#getPassword--) | Mendapatkan kata sandi. |
|
|  | [getCharset()](#getCharset--) | Mendapatkan enkoding dokumen. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Mendapatkan enkoding ANSI default yang digunakan untuk deteksi enkoding. |
|
|  | [getTimeout()](#getTimeout--) | Mendapatkan nilai yang mewakili jumlah milidetik untuk menunggu. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan timeout .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | batas waktu | java.time.Duration | Duration yang mewakili jumlah milidetik untuk menunggu. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan Password kosong, FileFormat sama dengan FileFormat.Unknown, dan enkoding default.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan FileFormat sama dengan FileFormat.Unknown dan enkoding default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan Password kosong dan enkoding default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Format file. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan enkoding default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Format file. |
|
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan enkoding khusus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Format file. |
|
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|
|  | charset | java.nio.charset.Charset | Enkoding dokumen. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Enkoding ANSI default yang digunakan untuk deteksi enkoding. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) yang sepenuhnya disesuaikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Format file. |
|
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|
|  | charset | java.nio.charset.Charset | Enkoding dokumen. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Enkoding ANSI default yang digunakan untuk deteksi enkoding. |
|
|  | batas waktu | java.time.Duration | Duration yang mewakili jumlah milidetik untuk menunggu. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan Password kosong dan enkoding default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Tipe file. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan kata sandi dan enkoding default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Tipe file. |
|
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dengan enkoding khusus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Tipe file. |
|
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|
|  | charset | java.nio.charset.Charset | Enkoding dokumen. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Enkoding ANSI default yang digunakan untuk deteksi enkoding. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Menginisialisasi instance baru dari kelas [LoadOptions](../../com.groupdocs.parser.options/loadoptions) yang sepenuhnya disesuaikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Tipe file. |
|
|  | kata sandi | java.lang.String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
|
|  | charset | java.nio.charset.Charset | Enkoding dokumen. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Enkoding ANSI default yang digunakan untuk deteksi enkoding. |
|
|  | batas waktu | java.time.Duration | Duration yang mewakili jumlah milidetik untuk menunggu. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Mendapatkan format file.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Mendapatkan tipe file.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Mendapatkan kata sandi.


**Returns:**
java.lang.String - Nilai string yang mewakili kata sandi untuk membuka file yang dilindungi kata sandi.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Mendapatkan enkoding dokumen.


**Returns:**
java.nio.charset.Charset - Sebuah instance dari kelas Charset yang mewakili enkoding dokumen; null jika tidak diatur.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Mendapatkan enkoding ANSI default yang digunakan untuk deteksi enkoding.


**Returns:**
java.nio.charset.Charset - Sebuah instance dari kelas Charset yang mewakili enkoding dokumen; null jika tidak diatur.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Mendapatkan nilai yang mewakili jumlah milidetik untuk menunggu.


**Returns:**
java.time.Duration - Sebuah instance dari Duration yang mewakili jumlah milidetik untuk menunggu.

