---
title: "PageAreaOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "페이지 영역 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 28
url: /ko/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

페이지 영역 추출에 사용되는 옵션을 제공합니다.

[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 클래스의 인스턴스는 [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-) 메서드의 매개변수로 사용됩니다.
및 [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) 메서드. 해당 사용 예제를 확인하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 클래스의 새 인스턴스를 무시되는 테두리 크기로 초기화합니다. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 페이지 영역을 포함하는 사각형 영역을 가져옵니다. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | 사각형 영역에 의해 캡처될 때 무시되는 테두리 크기를 가져옵니다. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 클래스의 새 인스턴스를 무시되는 테두리 크기로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 페이지 영역을 포함하는 사각형 영역입니다. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 페이지 영역을 포함하는 사각형 영역입니다. |
|
|  | rectangleTolerance | double | 사각형 영역에 의해 캡처될 때 무시되는 테두리 크기입니다. 텍스트 항목 높이의 비율로 측정됩니다. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


페이지 영역을 포함하는 사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


사각형 영역에 의해 캡처될 때 무시되는 테두리 크기를 가져옵니다. 텍스트 항목 높이의 비율로 측정됩니다.


**Returns:**
double - 0(테두리 없음)부터 1(전체 요소 무시)까지의 double 값.

