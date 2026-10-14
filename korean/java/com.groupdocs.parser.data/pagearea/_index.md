---
title: "PageArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 기반 파싱 기능에서 문서 페이지의 블록을 나타내는 데 사용되는 페이지 영역에 대한 추상 기본 클래스를 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

템플릿 기반 파싱 기능에서 문서 페이지의 블록을 나타내는 데 사용되는 페이지 영역에 대한 추상 기본 클래스를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 직사각형 영역을 가져옵니다. |
|
|  | [getPage()](#getPage--) | 페이지 인덱스 및 페이지 크기와 같은 문서 페이지 정보를 가져옵니다. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


직사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


페이지 인덱스 및 페이지 크기와 같은 문서 페이지 정보를 가져옵니다.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

