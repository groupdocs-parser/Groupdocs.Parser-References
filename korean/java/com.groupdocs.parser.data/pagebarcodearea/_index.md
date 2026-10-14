---
title: "PageBarcodeArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 기반 파싱 기능에서 바코드 값을 나타내는 페이지 바코드 영역을 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

템플릿 기반 파싱 기능에서 바코드 값을 나타내는 페이지 바코드 영역을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getValue()](#getValue--) | 바코드 값을 가져옵니다. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | 바코드 유형의 이름을 가져옵니다. |
|
|  | [getConfidence()](#getConfidence--) | 구문 분석된 바코드의 신뢰도 수준을 가져옵니다. |
|
|  | [getAngle()](#getAngle--) | 바코드의 각도를 가져옵니다. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


[PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 바코드의 값입니다. |
|
|  | codeTypeName | java.lang.String | 바코드의 유형 이름입니다. |
|
|  | confidence | int | 구문 분석된 바코드의 신뢰도 수준입니다. |
|
|  | angle | double | 바코드의 각도입니다. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 바코드 영역을 포함하는 페이지입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 바코드 영역을 포함하는 사각형 영역입니다. |
|

### getValue() {#getValue--}
```
public String getValue()
```


바코드 값을 가져옵니다.


**Returns:**
java.lang.String - 바코드 페이지 영역의 값을 나타내는 문자열 값입니다.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


바코드 유형의 이름을 가져옵니다.


**Returns:**
java.lang.String - 바코드의 유형 이름을 나타내는 문자열 값입니다.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


구문 분석된 바코드의 신뢰도 수준을 가져옵니다.


**Returns:**
int - 구문 분석된 바코드의 신뢰도를 나타내는 정수 값(0-100)입니다.

### getAngle() {#getAngle--}
```
public double getAngle()
```


바코드의 각도를 가져옵니다.


**Returns:**
double - 바코드의 각도를 나타내는 실수 값(0-360)입니다.

