---
title: "TemplateBarcode"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 바코드 필드를 제공합니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

템플릿 바코드 필드를 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | 새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | 새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스를 UPPER CASE 이름으로. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | 새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스를 UPPER CASE 이름으로. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | 새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 템플릿 바코드 필드를 포함하는 직사각형 영역을 가져옵니다. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 템플릿 바코드 필드를 포함하는 직사각형 영역입니다. |
|
|  | 이름 | java.lang.String | 바코드 필드 이름입니다. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스를 UPPER CASE 이름으로.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 템플릿 바코드 필드를 포함하는 직사각형 영역입니다. |
|
|  | 이름 | java.lang.String | 바코드 필드 이름입니다. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스를 UPPER CASE 이름으로.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 템플릿 바코드 필드를 포함하는 직사각형 영역입니다. |
|
|  | 이름 | java.lang.String | 바코드 필드 이름입니다. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 템플릿 바코드 필드를 포함하는 직사각형 영역입니다. |
|
|  | 이름 | java.lang.String | 바코드 필드 이름입니다. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


새 인스턴스를 초기화합니다 [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 템플릿 바코드 필드를 포함하는 직사각형 영역입니다. |
|
|  | 이름 | java.lang.String | 바코드 필드 이름입니다. |
|
|  | pageIndex | java.lang.Integer | 템플릿 항목이 위치한 페이지의 인덱스를 나타내는 정수 값; 템플릿 항목이 모든 페이지에 위치하는 경우  null  입니다. |
|
|  | pageWidth | java.lang.Double | 템플릿 항목을 만드는 데 사용된 페이지의 너비. |
|
|  | useUpperCaseName | boolean | name이 UPPER CASE로 변환되는지 여부를 나타내는 값. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


템플릿 바코드 필드를 포함하는 직사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

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
