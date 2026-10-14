---
title: "PageInfo"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "문서 페이지 정보를 나타냅니다."
type: docs
weight: 29
url: /ko/java/com.groupdocs.parser.options/pageinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageInfo
```

문서 페이지 정보를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageInfo(int pageNumber, int width, int height)](#PageInfo-int-int-int-) | 새로운 [PageInfo](../../com.groupdocs.parser.options/pageinfo) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 페이지 번호를 가져옵니다. |
|
|  | [getWidth()](#getWidth--) | 페이지 너비를 가져옵니다. |
|
|  | [getHeight()](#getHeight--) | 페이지 높이를 가져옵니다. |
|
### PageInfo(int pageNumber, int width, int height) {#PageInfo-int-int-int-}
```
public PageInfo(int pageNumber, int width, int height)
```


새로운 [PageInfo](../../com.groupdocs.parser.options/pageinfo) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageNumber | int | 페이지 번호. |
|
|  | 너비 | int | 페이지 너비. |
|
|  | 높이 | int | 페이지 높이. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


페이지 번호를 가져옵니다.


**Returns:**
int - 페이지 번호를 나타내는 0 기반 정수 값.

### getWidth() {#getWidth--}
```
public int getWidth()
```


페이지 너비를 가져옵니다.


**Returns:**
int - 페이지 너비를 나타내는 정수 값.

### getHeight() {#getHeight--}
```
public int getHeight()
```


페이지 높이를 가져옵니다.


**Returns:**
int - 페이지 높이를 나타내는 정수 값.

