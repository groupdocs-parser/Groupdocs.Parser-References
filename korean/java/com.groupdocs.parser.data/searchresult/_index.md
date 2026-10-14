---
title: "SearchResult"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "검색 기능에서 검색 결과를 나타냅니다."
type: docs
weight: 27
url: /ko/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

검색 기능에서 검색 결과를 나타냅니다.

SearchResult 클래스의 인스턴스는 [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-) 메서드의 반환값으로 사용됩니다.
그리고 [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) 메서드. 사용 예제는 해당 페이지를 참조하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | [SearchResult](../../com.groupdocs.parser.data/searchresult) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | [SearchResult](../../com.groupdocs.parser.data/searchresult) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPosition()](#getPosition--) | 문서 텍스트에서 위치를 가져옵니다. |
|
|  | [getText()](#getText--) | 텍스트를 가져옵니다. |
|
|  | [getPageIndex()](#getPageIndex--) | 텍스트가 발견된 페이지 인덱스를 가져옵니다. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | 왼쪽 하이라이트를 가져옵니다. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | 오른쪽 하이라이트를 가져옵니다. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


[SearchResult](../../com.groupdocs.parser.data/searchresult) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 위치 | int | 문서 텍스트 내 위치. |
|
|  | 텍스트 | java.lang.String | 찾은 텍스트. |
|
|  | pageIndex | java.lang.Integer | 텍스트가 발견된 페이지 인덱스. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | 왼쪽 하이라이트. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | 오른쪽 하이라이트. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


[SearchResult](../../com.groupdocs.parser.data/searchresult) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 위치 | int | 문서 텍스트 내 위치. |
|
|  | 텍스트 | java.lang.String | 찾은 텍스트. |
|
|  | pageIndex | java.lang.Integer | 텍스트가 발견된 페이지 인덱스. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


문서 텍스트에서 위치를 가져옵니다.


**Returns:**
int - 검색 결과 시작 위치의 0부터 시작하는 인덱스.

### getText() {#getText--}
```
public String getText()
```


텍스트를 가져옵니다.


**Returns:**
java.lang.String - 찾은 텍스트를 나타내는 문자열 값.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


텍스트가 발견된 페이지 인덱스를 가져옵니다.


**Returns:**
java.lang.Integer - 텍스트가 발견된 페이지의 0부터 시작하는 인덱스; 전체 문서 텍스트에 대해 검색이 수행된 경우  null  입니다.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


왼쪽 하이라이트를 가져옵니다.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


오른쪽 하이라이트를 가져옵니다.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

