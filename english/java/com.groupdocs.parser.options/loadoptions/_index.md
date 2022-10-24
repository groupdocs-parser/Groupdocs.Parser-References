---
title: LoadOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used to open a file.
type: docs
weight: 21
url: /java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Provides the options which are used to open a file.

An instance of this class is used as parameter in [Parser](../../com.groupdocs.parser/parser) class constructors:

 *  [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser\#Parser-java.io.InputStream--LoadOptions-)
 *  [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser\#Parser-String--LoadOptions-)

See the usage examples there.

**Learn more:**

 *  [Loading specific file formats][]
 *  [Password-protected documents][]


[Loading specific file formats]: https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats
[Password-protected documents]: https://docs.groupdocs.com/display/parserjava/Password-protected+documents
## Constructors

| Constructor | Description |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with empty  Password ,  FileFormat  equal to  FileFormat.Unknown  and default encodings. |
| [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with  FileFormat  equal to  FileFormat.Unknown  and default encodings. |
| [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with empty  Password  and default encodings. |
| [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with default encodings. |
| [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with custom encodings. |
## Methods

| Method | Description |
| --- | --- |
| [getFileFormat()](#getFileFormat--) | Gets the file format. |
| [getPassword()](#getPassword--) | Gets the password. |
| [getCharset()](#getCharset--) | Gets the encoding of the document. |
| [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Gets the default ANSI encoding which is used for encoding detection. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with empty  Password ,  FileFormat  equal to  FileFormat.Unknown  and default encodings.

### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with  FileFormat  equal to  FileFormat.Unknown  and default encodings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | The password to open the password-protected file. |

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with empty  Password  and default encodings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | The format of the file. |

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with default encodings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | The format of the file. |
| password | java.lang.String | The password to open the password-protected file. |

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Initializes a new instance of the [LoadOptions](../../com.groupdocs.parser.options/loadoptions) class with custom encodings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | The format of the file. |
| password | java.lang.String | The password to open the password-protected file. |
| charset | java.nio.charset.Charset | The encoding of the document. |
| defaultAnsiCharset | java.nio.charset.Charset | The default ANSI encoding which is used for encoding detection. |

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Gets the file format.

**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.
### getPassword() {#getPassword--}
```
public String getPassword()
```


Gets the password.

**Returns:**
java.lang.String - A string value that represents a password to open the password-protected file.
### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Gets the encoding of the document.

**Returns:**
java.nio.charset.Charset - An instance of  Charset  class that represents the document encoding;  null  if it isn't set.
### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Gets the default ANSI encoding which is used for encoding detection.

**Returns:**
java.nio.charset.Charset - An instance of  Charset  class that represents the document encoding;  null  if it isn't set.
