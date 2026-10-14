---
title: "TemplateItem"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 항목을 위한 기본 추상 클래스를 제공합니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

템플릿 항목을 위한 기본 추상 클래스를 제공합니다.

[TemplateItem](../../com.groupdocs.parser.templates/templateitem) 클래스의 상속자는 [Template](../../com.groupdocs.parser.templates/template) 컬렉션에서 사용됩니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | 주어진 계수를 사용하여 모든 좌표를 스케일링한 현재 항목의 복사본을 생성합니다. |
|
|  | [getName()](#getName--) | 템플릿 항목의 이름을 가져옵니다. |
|
|  | [getPageIndex()](#getPageIndex--) | 템플릿 항목의 페이지 인덱스를 가져옵니다. |
|
|  | [getPageWidth()](#getPageWidth--) | 템플릿 항목을 만드는 데 사용된 페이지의 너비를 가져옵니다. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Name이 대문자로 변환되었는지 여부를 나타내는 값을 가져옵니다. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


주어진 계수를 사용하여 모든 좌표를 스케일링한 현재 항목의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | factor | double | 스케일링 계수. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


템플릿 항목의 이름을 가져옵니다.


**Returns:**
java.lang.String - 템플릿 항목의 이름을 나타내는 대문자 문자열 값.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


템플릿 항목의 페이지 인덱스를 가져옵니다.


**Returns:**
java.lang.Integer - 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


템플릿 항목을 만드는 데 사용된 페이지의 너비를 가져옵니다.


**Returns:**
java.lang.Double - 페이지의 너비(픽셀 단위); 페이지 너비를 알 수 없는 경우  null  입니다.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Name이 대문자로 변환되었는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - Name이 대문자로 변환되었는지 여부를 나타내는 부울 값.

