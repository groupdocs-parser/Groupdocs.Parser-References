---
title: "FileTypeDetectionMode"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "파일 유형 감지 모드를 정의합니다."
type: docs
weight: 44
url: /ko/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

파일 유형 감지 모드를 정의합니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Default](#Default) | 파일 유형은 파일 확장자를 통해 감지됩니다; 파일 확장자를 인식하지 못하면 파일 내용을 통해 감지됩니다. |
|
|  | [Extension](#Extension) | 파일 유형은 파일 확장자만으로 감지됩니다. |
|
|  | [Content](#Content) | 파일 유형은 파일 내용만으로 감지됩니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


파일 유형은 파일 확장자를 통해 감지됩니다; 파일 확장자를 인식하지 못하면 파일 내용을 통해 감지됩니다.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


파일 유형은 파일 확장자만으로 감지됩니다.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


파일 유형은 파일 내용만으로 감지됩니다.


### values() {#values--}
```
public static FileTypeDetectionMode[] values()
```




**Returns:**
com.groupdocs.parser.options.FileTypeDetectionMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileTypeDetectionMode valueOf(String name)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)
