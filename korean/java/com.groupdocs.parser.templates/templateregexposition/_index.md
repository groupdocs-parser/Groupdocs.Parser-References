---
title: "TemplateRegexPosition"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "정규식을 사용하는 템플릿 필드 위치를 제공합니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

정규식을 사용하는 템플릿 필드 위치를 제공합니다.

다음 예제는 문서에 "Invoice Number INV-12345"가 포함된 경우를 보여줍니다.
그런 다음 템플릿 필드를 다음과 같이 정의할 수 있습니다:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

이 경우 값으로 전체 문자열이 추출됩니다. 문자열의 일부만 추출하려면
정규식 그룹 "value"를 사용합니다:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

이 경우 값으로 "INV-3337" 문자열이 추출됩니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | 새로운 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 클래스 인스턴스를 초기화합니다. |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | 새로운 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getExpression()](#getExpression--) | 정규식을 가져옵니다. |
|
|  | [isMatchCase()](#isMatchCase--) | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값을 가져옵니다. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


새로운 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


새로운 [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


정규식을 가져옵니다.


**Returns:**
java.lang.String - 정규식을 나타내는 문자열입니다.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 텍스트 대소문자를 무시하지 않으면 true, 그렇지 않으면 false.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


주어진 factor에 따라 모든 좌표를 스케일링한 현재 위치의 복사본을 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
