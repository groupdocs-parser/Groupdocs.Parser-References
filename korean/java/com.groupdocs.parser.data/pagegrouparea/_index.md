---
title: "PageGroupArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 기반 파싱 기능에서 문서 페이지의 다양한 유형 블록을 그룹화하는 데 사용되는 페이지 영역 그룹을 나타냅니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

템플릿 기반 파싱 기능에서 문서 페이지의 다양한 유형 블록을 그룹화하는 데 사용되는 페이지 영역 그룹을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getAreas()](#getAreas--) | 그룹화된 페이지 영역 컬렉션을 가져옵니다. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


[PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 영역 | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | 그룹화될 페이지 영역 컬렉션. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 해당 영역을 포함하는 페이지. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


그룹화된 페이지 영역 컬렉션을 가져옵니다.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - [PageArea](../../com.groupdocs.parser.data/pagearea) 객체의 컬렉션.

