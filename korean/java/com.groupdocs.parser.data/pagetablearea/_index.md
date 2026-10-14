---
title: "PageTableArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 기반 파싱 기능에서 테이블을 나타내는 테이블 페이지 영역을 나타냅니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

템플릿 기반 파싱 기능에서 테이블을 나타내는 테이블 페이지 영역을 나타냅니다.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 새로운 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCells()](#getCells--) | 셀 컬렉션을 가져옵니다. |
|
|  | [getRowCount()](#getRowCount--) | 테이블 행의 총 개수를 가져옵니다. |
|
|  | [getColumnCount()](#getColumnCount--) | 테이블 열의 총 개수를 가져옵니다. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | 행 높이를 반환합니다. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | 열 너비를 반환합니다. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | 행 및 열 인덱스로 테이블 셀을 가져옵니다. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


새로운 [PageTableArea](../../com.groupdocs.parser.data/pagetablearea) 클래스 인스턴스를 초기화합니다.

참고: C# 프로젝트는 이 생성자를 다음과 같이 표시합니다
internal
(commit 954951f). Java에서는 "internal-to-the-assembly"
패키지-프라이빗으로 깔끔하게 변환되지 않습니다. 왜냐하면 생산자(
WordProcessingParser
,
TableAreaParser
,
etc.) 은 다음에 존재합니다
com.groupdocs.parser
, 가 아니라
com.groupdocs.parser.data
. 따라서 생성자는 유지됩니다

public
그래서 패키지 간 생성이 여전히 작동합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 행 | java.lang.Iterable<java.lang.Double> | 행 높이의 컬렉션입니다. |
|
|  | 열 | java.lang.Iterable<java.lang.Double> | 열 너비의 컬렉션입니다. |
|
|  | 셀 | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | 셀의 컬렉션입니다. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 테이블을 포함하는 페이지입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 표를 포함하는 직사각형 영역입니다. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


셀 컬렉션을 가져옵니다. 테이블 셀의 단순 읽기 전용 컬렉션입니다.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - 테이블 셀의 컬렉션

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


테이블 행의 총 개수를 가져옵니다.


**Returns:**
int - 테이블 행의 총 수를 포함하는 정수 값입니다.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


테이블 열의 총 개수를 가져옵니다.


**Returns:**
int - 테이블 열의 총 수를 포함하는 정수 값입니다.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


행 높이를 반환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rowIndex | int | 행의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
double - 행의 높이를 나타내는 실수 값입니다.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


열 너비를 반환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | columnIndex | int | 열의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
double - 열의 너비를 나타내는 실수 값입니다.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


행 및 열 인덱스로 테이블 셀을 가져옵니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rowIndex | int | 셀 행의 0부터 시작하는 인덱스입니다. |
|
|  | columnIndex | int | 셀 열의 0부터 시작하는 인덱스입니다. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

