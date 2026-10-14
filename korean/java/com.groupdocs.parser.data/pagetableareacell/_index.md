---
title: "PageTableAreaCell"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "클래스에서 사용되는 테이블 셀을 나타냅니다."
type: docs
weight: 23
url: /ko/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 클래스에서 사용되는 테이블 셀을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | 행 인덱스를 가져옵니다. |
|
|  | [getColumnIndex()](#getColumnIndex--) | 열 인덱스를 가져옵니다. |
|
|  | [getRowSpan()](#getRowSpan--) | 테이블 셀을 포함하는 전체 행 수를 가져옵니다. |
|
|  | [getColumnSpan()](#getColumnSpan--) | 테이블 셀을 포함하는 전체 열 수를 가져옵니다. |
|
|  | [getPageArea()](#getPageArea--) | 테이블 셀 값을 가져옵니다. |
|
|  | [getText()](#getText--) | 테이블 셀 텍스트 값을 가져옵니다. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rowIndex | int | 행의 0부터 시작하는 인덱스입니다. |
|
|  | columnIndex | int | 열의 0부터 시작하는 인덱스입니다. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | 표 셀의 값입니다. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rowIndex | int | 행의 0부터 시작하는 인덱스입니다. |
|
|  | columnIndex | int | 열의 0부터 시작하는 인덱스입니다. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | 표 셀의 값입니다. |
|
|  | rowSpan | int | 표 셀을 포함하는 행의 총 수입니다. |
|
|  | columnSpan | int | 표 셀을 포함하는 열의 총 수입니다. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


행 인덱스를 가져옵니다.


**Returns:**
int - 표 셀을 포함하는 첫 번째 행의 0부터 시작하는 인덱스입니다.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


열 인덱스를 가져옵니다.


**Returns:**
int - 표 셀을 포함하는 첫 번째 열의 0부터 시작하는 인덱스입니다.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


테이블 셀을 포함하는 전체 행 수를 가져옵니다.


**Returns:**
int - 표 셀을 포함하는 행의 총 수를 나타내는 양의 정수 값입니다.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


테이블 셀을 포함하는 전체 열 수를 가져옵니다.


**Returns:**
int - 표 셀을 포함하는 열의 총 수를 나타내는 양의 정수 값입니다.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


테이블 셀 값을 가져옵니다.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


테이블 셀 텍스트 값을 가져옵니다.


**Returns:**
java.lang.String - 셀의 텍스트 값을 나타내는 문자열이며, 셀에 텍스트 값이 없으면 null입니다.

