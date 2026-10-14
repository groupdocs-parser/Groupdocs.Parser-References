---
title: "TemplateField"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 텍스트 필드를 제공합니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

템플릿 텍스트 필드를 제공합니다.

텍스트 필드는 페이지상의 위치에 따라 정의됩니다. 텍스트 필드를 정의하는 방법은 세 가지가 있습니다:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | 대문자 이름으로 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | 대문자 이름으로 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getPosition()](#getPosition--) | 문서 페이지에서 템플릿 필드를 찾는 방법을 설명하는 값을 가져옵니다. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 필드 위치. |
|
|  | 이름 | java.lang.String | 필드 이름. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


대문자 이름으로 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 필드 위치. |
|
|  | 이름 | java.lang.String | 필드 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


대문자 이름으로 새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 필드 위치. |
|
|  | 이름 | java.lang.String | 필드 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 필드 위치. |
|
|  | 이름 | java.lang.String | 필드 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


새로운 [TemplateField](../../com.groupdocs.parser.templates/templatefield) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | 필드 위치. |
|
|  | 이름 | java.lang.String | 필드 이름. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


문서 페이지에서 템플릿 필드를 찾는 방법을 설명하는 값을 가져옵니다.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


주어진 계수를 사용하여 모든 좌표를 스케일링한 현재 항목의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
