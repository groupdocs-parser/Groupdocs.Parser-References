---
title: "PageRenderInfo"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "페이지가 렌더링되는 방식에 대한 정보를 나타냅니다."
type: docs
weight: 30
url: /ko/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

페이지가 렌더링되는 방식에 대한 정보를 나타냅니다.

일부 문서(예: 스프레드시트)는 페이지를 렌더링할 수 없습니다
단일 이미지로. 이러한 문서의 경우 페이지가 타일 집합으로 렌더링됩니다.
이 타일들은 직사각형 테이블에 배치됩니다.


RowCount
및
ColumnCount
행과 열의 총 수를 나타냅니다
이 테이블의. 문서 페이지가 단일 이미지로 렌더링되면 이러한 속성은 1이 됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | 새 인스턴스를 초기화합니다 [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) 클래스. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 페이지 번호를 가져옵니다. |
|
|  | [getRowCount()](#getRowCount--) | 타일 행의 총 수를 가져옵니다. |
|
|  | [getColumnCount()](#getColumnCount--) | 타일 열의 총 수를 가져옵니다. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | tileIndex를 가진 타일이 배치된 열의 인덱스를 반환합니다. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | tileIndex를 가진 타일이 배치된 행의 인덱스를 반환합니다. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


새 인스턴스를 초기화합니다 [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageNumber | int | 페이지 번호(1부터 시작합니다). |
|
|  | rowCount | int | 타일 행의 총 개수. |
|
|  | columnCount | int | 타일 열의 총 개수. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


페이지 번호를 가져옵니다.


**Returns:**
int - 페이지 번호를 나타내는 정수 값(1부터 시작합니다).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


타일 행의 총 수를 가져옵니다.


**Returns:**
int - 타일 행의 총 개수를 나타내는 정수 값.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


타일 열의 총 수를 가져옵니다.


**Returns:**
int - 타일 열의 총 개수를 나타내는 정수 값.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


tileIndex를 가진 타일이 배치된 열의 인덱스를 반환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | tileIndex | int | 타일의 0 기반 인덱스. |
|

**Returns:**
int - 열 인덱스를 나타내는 0 기반 정수 값.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


tileIndex를 가진 타일이 배치된 행의 인덱스를 반환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | tileIndex | int | 타일의 0 기반 인덱스. |
|

**Returns:**
int - 행 인덱스를 나타내는 0 기반 정수 값.

