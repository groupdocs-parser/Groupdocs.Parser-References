---
title: "LoadOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для открытия файла."
type: docs
weight: 24
url: /ru/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Предоставляет параметры, используемые для открытия файла.

Экземпляр этого класса используется в качестве параметра в конструкторах класса [Parser](../../com.groupdocs.parser/parser):

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Смотрите примеры использования там.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с тайм‑аутом. |
|
|  | [LoadOptions()](#LoadOptions--) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пустым Password, FileFormat, равным FileFormat.Unknown, и кодировками по умолчанию. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с FileFormat, равным FileFormat.Unknown, и кодировками по умолчанию. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пустым Password и кодировками по умолчанию. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с кодировками по умолчанию. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пользовательскими кодировками. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Инициализирует новый экземпляр полностью настроенного класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пустым Password и кодировками по умолчанию. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с паролем и кодировками по умолчанию. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пользовательскими кодировками. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Инициализирует новый экземпляр полностью настроенного класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Получает формат файла. |
|
|  | [getFileType()](#getFileType--) | Получает тип файла. |
|
|  | [getPassword()](#getPassword--) | Получает пароль. |
|
|  | [getCharset()](#getCharset--) | Получает кодировку документа. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Получает кодировку ANSI по умолчанию, используемую для обнаружения кодировки. |
|
|  | [getTimeout()](#getTimeout--) | Получает значение, представляющее количество миллисекунд ожидания. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с тайм‑аутом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | тайм-аут | java.time.Duration | Продолжительность Duration, представляющая количество миллисекунд ожидания. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пустым Password, FileFormat, равным FileFormat.Unknown, и кодировками по умолчанию.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с FileFormat, равным FileFormat.Unknown, и кодировками по умолчанию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пустым Password и кодировками по умолчанию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Формат файла. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с кодировками по умолчанию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Формат файла. |
|
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пользовательскими кодировками.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Формат файла. |
|
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|
|  | charset | java.nio.charset.Charset | Кодировка документа. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Кодировка ANSI по умолчанию, используемая для обнаружения кодировки. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Инициализирует новый экземпляр полностью настроенного класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Формат файла. |
|
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|
|  | charset | java.nio.charset.Charset | Кодировка документа. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Кодировка ANSI по умолчанию, используемая для обнаружения кодировки. |
|
|  | тайм-аут | java.time.Duration | Продолжительность Duration, представляющая количество миллисекунд ожидания. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пустым Password и кодировками по умолчанию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Тип файла. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с паролем и кодировками по умолчанию.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Тип файла. |
|
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Инициализирует новый экземпляр класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions) с пользовательскими кодировками.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Тип файла. |
|
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|
|  | charset | java.nio.charset.Charset | Кодировка документа. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Кодировка ANSI по умолчанию, используемая для обнаружения кодировки. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Инициализирует новый экземпляр полностью настроенного класса [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Тип файла. |
|
|  | пароль | java.lang.String | Пароль для открытия файла, защищённого паролем. |
|
|  | charset | java.nio.charset.Charset | Кодировка документа. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Кодировка ANSI по умолчанию, используемая для обнаружения кодировки. |
|
|  | тайм-аут | java.time.Duration | Продолжительность Duration, представляющая количество миллисекунд ожидания. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Получает формат файла.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Получает тип файла.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Получает пароль.


**Returns:**
java.lang.String - Строковое значение, представляющее пароль для открытия файла, защищённого паролем.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Получает кодировку документа.


**Returns:**
java.nio.charset.Charset - Экземпляр класса Charset, представляющий кодировку документа; null, если она не установлена.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Получает кодировку ANSI по умолчанию, используемую для обнаружения кодировки.


**Returns:**
java.nio.charset.Charset - Экземпляр класса Charset, представляющий кодировку документа; null, если она не установлена.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Получает значение, представляющее количество миллисекунд ожидания.


**Returns:**
java.time.Duration - Экземпляр Duration, представляющий количество миллисекунд ожидания.

