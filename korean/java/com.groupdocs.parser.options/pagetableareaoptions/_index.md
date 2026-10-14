---
title: "PageTableAreaOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "페이지 표 영역 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 31
url: /ko/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

페이지 표 영역 추출에 사용되는 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 클래스의 새 인스턴스를 검색 사각형과 고정 레이아웃 없이 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | 페이지에서 테이블을 정의하는 테이블 레이아웃을 가져옵니다. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


[PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | 페이지에서 테이블을 정의하는 테이블 레이아웃. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


[PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) 클래스의 새 인스턴스를 검색 사각형과 고정 레이아웃 없이 초기화합니다.

페이지 영역에 자동 감지된 테이블을 제한하는 데 유용합니다. C#을 반영합니다.

new PageTableAreaOptions(null) { Rectangle = ... }
패턴.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 테이블을 감지해야 하는 페이지의 사각형 영역; 전체 페이지를 검색하려면 null을 전달합니다. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


페이지에서 테이블을 정의하는 테이블 레이아웃을 가져옵니다.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

