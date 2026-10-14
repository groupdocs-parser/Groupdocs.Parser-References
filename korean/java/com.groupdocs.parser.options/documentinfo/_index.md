---
title: "DocumentInfo"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "문서 정보를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

문서 정보를 나타냅니다.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 문서 유형을 가져옵니다. |
|
|  | [getPageCount()](#getPageCount--) | 문서 페이지의 총 수를 가져옵니다. |
|
|  | [getRawPageCount()](#getRawPageCount--) | 문서 원시 페이지의 총 수를 가져옵니다. |
|
|  | [getSize()](#getSize--) | 문서의 크기를 바이트 단위로 가져옵니다. |
|
|  | [getPages()](#getPages--) | 페이지의 인덱스 및 페이지 크기와 같은 정보를 가져옵니다. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


문서 유형을 가져옵니다.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


문서 페이지의 총 수를 가져옵니다.


**Returns:**
int - 페이지 총 수를 나타내는 정수 값입니다.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


문서 원시 페이지의 총 수를 가져옵니다.

원시 텍스트 추출을 위해 [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) 속성을 사용하고, [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) 속성을 대신 사용하십시오.
일부 문서는 정확한 텍스트 추출 모드와 원시 텍스트 추출 모드에서 페이지 번호가 다를 수 있습니다.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - 원시 페이지 총 수를 나타내는 정수 값입니다.

### getSize() {#getSize--}
```
public abstract long getSize()
```


문서의 크기를 바이트 단위로 가져옵니다.


**Returns:**
long - 문서의 크기를 바이트 단위로 나타내는 정수 값.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


페이지의 인덱스 및 페이지 크기와 같은 정보를 가져옵니다.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - [PageInfo](../../com.groupdocs.parser.options/pageinfo) 클래스 인스턴스들의 컬렉션입니다.

