---
title: "TemplateOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 기능을 통한 구문 분석에 사용되는 옵션을 제공합니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

템플릿 기능을 통한 구문 분석에 사용되는 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | 새로운 [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | 사각형 영역에 의해 캡처될 때 무시되는 테두리 크기를 가져옵니다. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


새로운 [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangleTolerance | double | 사각형 영역에 의해 캡처될 때 무시되는 테두리 크기입니다. 텍스트 항목 높이의 비율로 측정됩니다. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


사각형 영역에 의해 캡처될 때 무시되는 테두리 크기를 가져옵니다. 텍스트 항목 높이의 비율로 측정됩니다.


**Returns:**
double - 0(테두리 없음)부터 1(전체 요소 무시)까지의 double 값.

