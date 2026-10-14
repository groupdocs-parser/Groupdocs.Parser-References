---
title: "PageHyperlinkArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "페이지의 하이퍼링크를 나타내는 페이지 영역을 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

페이지의 하이퍼링크를 나타내는 페이지 영역을 나타냅니다.

다음 메서드들의 반환 값으로 [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 클래스의 인스턴스가 사용됩니다.

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

그곳의 사용 예제를 확인하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getText()](#getText--) | 하이퍼링크 텍스트를 가져옵니다. |
|
|  | [getUrl()](#getUrl--) | 하이퍼링크 URL을 가져옵니다. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


[PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 텍스트 | java.lang.String | 하이퍼링크 텍스트입니다. |
|
|  | url | java.lang.String | 하이퍼링크 URL입니다. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 하이퍼링크를 포함하는 페이지입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 하이퍼링크를 포함하는 사각형 영역입니다. |
|

### getText() {#getText--}
```
public String getText()
```


하이퍼링크 텍스트를 가져옵니다.


**Returns:**
java.lang.String - 하이퍼링크 텍스트를 나타내는 문자열 값입니다.

### getUrl() {#getUrl--}
```
public String getUrl()
```


하이퍼링크 URL을 가져옵니다.


**Returns:**
java.lang.String - 하이퍼링크 URL을 나타내는 문자열 값입니다.

