---
title: "PageTextArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 파싱 또는 양식 파싱 기능에서 텍스트 값을 나타내는 페이지 텍스트 영역을 나타냅니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

템플릿 파싱 또는 양식 파싱 기능에서 텍스트 값을 나타내는 페이지 텍스트 영역을 나타냅니다.

다음 메서드의 반환값으로 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스의 인스턴스가 사용됩니다:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

또한 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스의 인스턴스가 [PageArea](../../com.groupdocs.parser.data/pagearea) 속성의 값으로 사용됩니다.
\\*

그곳의 사용 예제를 확인하십시오.

텍스트 영역은 단일이거나 복합일 수 있습니다. 첫 번째 경우에는 직사각형 영역으로 제한된 텍스트를 포함합니다.
두 번째 경우에는 다른 텍스트 영역을 포함합니다; 텍스트 및 테이블 속성은 하위 텍스트 영역에 의해 계산됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 새로운 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스 인스턴스를 초기화합니다. |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 새로운 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스 인스턴스를 초기화합니다. |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | 새로운 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getText()](#getText--) | 텍스트를 가져옵니다. |
|
|  | [getBaseLine()](#getBaseLine--) | 기준선을 가져옵니다. |
|
|  | [getTextStyle()](#getTextStyle--) | 글꼴 크기, 글꼴 이름 등과 같은 텍스트 스타일을 가져옵니다. |
|
|  | [getAreas()](#getAreas--) | 자식 텍스트 페이지 영역의 컬렉션을 가져옵니다. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


새로운 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 텍스트 | java.lang.String | 텍스트의 값입니다. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 텍스트 영역을 포함하는 페이지입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 텍스트 영역을 포함하는 직사각형 영역입니다. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


새로운 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 텍스트 | java.lang.String | 텍스트의 값입니다. |
|
|  | baseLine | java.lang.Double | 텍스트의 베이스라인입니다. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | 텍스트의 스타일입니다. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 텍스트 영역을 포함하는 페이지입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 텍스트 영역을 포함하는 직사각형 영역입니다. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


새로운 [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 영역 | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 자식 텍스트 페이지 영역의 컬렉션입니다. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 텍스트 영역을 포함하는 페이지입니다. |
|

### getText() {#getText--}
```
public String getText()
```


텍스트를 가져옵니다.


**Returns:**
java.lang.String - 텍스트 페이지 영역의 값을 나타내는 문자열 값입니다.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


기준선을 가져옵니다.


**Returns:**
double - 베이스라인을 나타내는 double 값입니다.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


글꼴 크기, 글꼴 이름 등과 같은 텍스트 스타일을 가져옵니다.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


자식 텍스트 페이지 영역의 컬렉션을 가져옵니다.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - 자식 텍스트 페이지 영역의 컬렉션입니다; 텍스트 페이지 영역에 자식이 없으면 비어 있습니다.

