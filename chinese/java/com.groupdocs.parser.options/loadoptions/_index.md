---
title: "LoadOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于打开文件的选项。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

提供用于打开文件的选项。

此类的实例用作 [Parser](../../com.groupdocs.parser/parser) 类构造函数的参数：

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

请参阅那里的使用示例。

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | 使用 timeout 初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions()](#LoadOptions--) | 使用空的 Password、FileFormat 等于 FileFormat.Unknown 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | 使用 FileFormat 等于 FileFormat.Unknown 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | 使用空的 Password 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | 使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | 使用自定义编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | 初始化完全自定义的 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的实例。 |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | 使用空的 Password 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | 使用密码和默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | 使用自定义编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。 |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | 初始化完全自定义的 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | 获取文件格式。 |
|
|  | [getFileType()](#getFileType--) | 获取文件类型。 |
|
|  | [getPassword()](#getPassword--) | 获取密码。 |
|
|  | [getCharset()](#getCharset--) | 获取文档的编码。 |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | 获取用于编码检测的默认 ANSI 编码。 |
|
|  | [getTimeout()](#getTimeout--) | 获取表示等待毫秒数的值。 |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


使用 timeout 初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 超时 | java.time.Duration | 表示等待毫秒数的 Duration。 |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


使用空的 Password、FileFormat 等于 FileFormat.Unknown 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


使用 FileFormat 等于 FileFormat.Unknown 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


使用空的 Password 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 文件的格式。 |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 文件的格式。 |
|
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


使用自定义编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 文件的格式。 |
|
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|
|  | 字符集 | java.nio.charset.Charset | 文档的编码。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 用于编码检测的默认 ANSI 编码。 |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


初始化完全自定义的 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 文件的格式。 |
|
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|
|  | 字符集 | java.nio.charset.Charset | 文档的编码。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 用于编码检测的默认 ANSI 编码。 |
|
|  | 超时 | java.time.Duration | 表示等待毫秒数的 Duration。 |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


使用空的 Password 并使用默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 文件的类型。 |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


使用密码和默认编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 文件的类型。 |
|
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


使用自定义编码初始化 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 文件的类型。 |
|
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|
|  | 字符集 | java.nio.charset.Charset | 文档的编码。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 用于编码检测的默认 ANSI 编码。 |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


初始化完全自定义的 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 类的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 文件的类型。 |
|
|  | 密码 | java.lang.String | 打开受密码保护的文件所需的密码。 |
|
|  | 字符集 | java.nio.charset.Charset | 文档的编码。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 用于编码检测的默认 ANSI 编码。 |
|
|  | 超时 | java.time.Duration | 表示等待毫秒数的 Duration。 |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


获取文件格式。


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


获取文件类型。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


获取密码。


**Returns:**
java.lang.String - 表示打开受密码保护的文件的密码的字符串值。

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


获取文档的编码。


**Returns:**
java.nio.charset.Charset - 表示文档编码的 Charset 类的实例；如果未设置则为 null。

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


获取用于编码检测的默认 ANSI 编码。


**Returns:**
java.nio.charset.Charset - 表示文档编码的 Charset 类的实例；如果未设置则为 null。

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


获取表示等待毫秒数的值。


**Returns:**
java.time.Duration - 表示等待毫秒数的 Duration 实例。

