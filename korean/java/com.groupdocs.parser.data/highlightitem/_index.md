---
title: "HighlightItem"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트의 일부를 강조 표시하며, 검색 기능에서 찾은 텍스트의 컨텍스트를 설명하는 데 일반적으로 사용됩니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

검색 기능에서 찾은 텍스트의 컨텍스트를 설명하는 데 일반적으로 사용되는 텍스트의 일부인 하이라이트를 나타냅니다.

[HighlightItem](../../com.groupdocs.parser.data/highlightitem) 클래스의 인스턴스는 [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) 메서드의 반환값으로 사용됩니다.
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPosition()](#getPosition--) | 문서 텍스트에서 위치를 가져옵니다. |
|
|  | [getText()](#getText--) | 강조 표시된 텍스트를 가져옵니다. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


[HighlightItem](../../com.groupdocs.parser.data/highlightitem) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 위치 | int | 문서 텍스트 내 위치. |
|
|  | 텍스트 | java.lang.String | 강조된 텍스트. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


문서 텍스트에서 위치를 가져옵니다.


**Returns:**
int - 강조 표시 시작 위치의 0부터 시작하는 인덱스.

### getText() {#getText--}
```
public String getText()
```


강조 표시된 텍스트를 가져옵니다.


**Returns:**
java.lang.String - 강조된 텍스트를 나타내는 문자열 값.

