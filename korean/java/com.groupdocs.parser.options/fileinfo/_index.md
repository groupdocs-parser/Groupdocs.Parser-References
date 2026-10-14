---
title: "FileInfo"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "파일 정보를 나타냅니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

파일 정보를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 문서 유형을 가져옵니다. |
|
|  | [getSize()](#getSize--) | 문서의 크기를 바이트 단위로 가져옵니다. |
|
|  | [isEncrypted()](#isEncrypted--) | 파일이 비밀번호로 보호되는지를 나타내는 값을 가져옵니다. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


문서 유형을 가져옵니다.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


문서의 크기를 바이트 단위로 가져옵니다.


**Returns:**
long - 문서의 크기를 바이트 단위로 나타내는 정수 값.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


파일이 비밀번호로 보호되는지를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 파일이 비밀번호로 보호되는 경우 true; 그렇지 않으면 false.

