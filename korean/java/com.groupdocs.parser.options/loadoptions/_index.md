---
title: "LoadOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "파일을 열 때 사용되는 옵션을 제공합니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

파일을 열 때 사용되는 옵션을 제공합니다.

이 클래스의 인스턴스는 [Parser](../../com.groupdocs.parser/parser) 클래스 생성자에서 매개변수로 사용됩니다:

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

그곳의 사용 예제를 확인하십시오.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 timeout과 함께 초기화합니다. |
|
|  | [LoadOptions()](#LoadOptions--) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 빈 Password, FileFormat이 FileFormat.Unknown와 동일하고 기본 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 FileFormat이 FileFormat.Unknown와 동일하고 기본 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 빈 Password와 기본 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 기본 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 사용자 지정 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | 완전히 사용자 지정된 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스를 초기화합니다. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 빈 Password와 기본 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | 비밀번호와 기본 인코딩을 사용하여 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | 새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 사용자 지정 인코딩과 함께 초기화합니다. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | 완전히 사용자 지정된 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | 파일 형식을 가져옵니다. |
|
|  | [getFileType()](#getFileType--) | 파일 유형을 가져옵니다. |
|
|  | [getPassword()](#getPassword--) | 비밀번호를 가져옵니다. |
|
|  | [getCharset()](#getCharset--) | 문서의 인코딩을 가져옵니다. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | 인코딩 감지에 사용되는 기본 ANSI 인코딩을 가져옵니다. |
|
|  | [getTimeout()](#getTimeout--) | 대기할 밀리초 수를 나타내는 값을 가져옵니다. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 timeout과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | timeout | java.time.Duration | 대기할 밀리초 수를 나타내는 Duration입니다. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 빈 Password, FileFormat이 FileFormat.Unknown와 동일하고 기본 인코딩과 함께 초기화합니다.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 FileFormat이 FileFormat.Unknown와 동일하고 기본 인코딩과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 빈 Password와 기본 인코딩과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 파일의 형식입니다. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 기본 인코딩과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 파일의 형식입니다. |
|
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 사용자 지정 인코딩과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 파일의 형식입니다. |
|
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|
|  | charset | java.nio.charset.Charset | 문서의 인코딩입니다. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


완전히 사용자 지정된 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | 파일의 형식입니다. |
|
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|
|  | charset | java.nio.charset.Charset | 문서의 인코딩입니다. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |
|
|  | timeout | java.time.Duration | 대기할 밀리초 수를 나타내는 Duration입니다. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 빈 Password와 기본 인코딩과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 파일의 유형입니다. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


비밀번호와 기본 인코딩을 사용하여 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 파일의 유형입니다. |
|
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


새로운 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스 인스턴스를 사용자 지정 인코딩과 함께 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 파일의 유형입니다. |
|
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|
|  | charset | java.nio.charset.Charset | 문서의 인코딩입니다. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


완전히 사용자 지정된 [LoadOptions](../../com.groupdocs.parser.options/loadoptions) 클래스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 파일의 유형입니다. |
|
|  | 비밀번호 | java.lang.String | 암호가 보호된 파일을 열기 위한 비밀번호입니다. |
|
|  | charset | java.nio.charset.Charset | 문서의 인코딩입니다. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | 인코딩 감지에 사용되는 기본 ANSI 인코딩입니다. |
|
|  | timeout | java.time.Duration | 대기할 밀리초 수를 나타내는 Duration입니다. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


파일 형식을 가져옵니다.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


파일 유형을 가져옵니다.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


비밀번호를 가져옵니다.


**Returns:**
java.lang.String - 암호가 보호된 파일을 열기 위한 비밀번호를 나타내는 문자열 값입니다.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


문서의 인코딩을 가져옵니다.


**Returns:**
java.nio.charset.Charset - 문서 인코딩을 나타내는 Charset 클래스의 인스턴스; 설정되지 않은 경우 null입니다.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


인코딩 감지에 사용되는 기본 ANSI 인코딩을 가져옵니다.


**Returns:**
java.nio.charset.Charset - 문서 인코딩을 나타내는 Charset 클래스의 인스턴스; 설정되지 않은 경우 null입니다.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


대기할 밀리초 수를 나타내는 값을 가져옵니다.


**Returns:**
java.time.Duration - 대기할 밀리초 수를 나타내는 Duration의 인스턴스입니다.

