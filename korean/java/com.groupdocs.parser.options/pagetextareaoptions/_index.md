---
title: "PageTextAreaOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "페이지 텍스트 영역 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 32
url: /ko/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

페이지 텍스트 영역 추출에 사용되는 옵션을 제공합니다.

[PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스는 [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-) 메서드의 매개변수로 사용됩니다.
그리고 [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) 메서드. 해당 예제들을 확인하십시오.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | 기본값으로 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | OCR 사용 옵션과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | OCR 옵션을 설정할 수 있는 기능과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | 정규식으로 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | 정규식 및 사각형 영역으로 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | 정규식, 사각형 영역 및 무시된 테두리 크기로 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | 새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | 무시된 테두리 크기를 지정하여 새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getExpression()](#getExpression--) | 정규식을 가져옵니다. |
|
|  | [isMatchCase()](#isMatchCase--) | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isUniteSegments()](#isUniteSegments--) | 세그먼트가 결합되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | 텍스트 서식이 무시되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isUseOcr()](#isUseOcr--) | 텍스트 추출에 OCR 커넥터가 사용되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR 기능에 대한 추가 옵션을 가져옵니다. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


기본값으로 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


OCR 사용 옵션과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | useOcr | boolean | 텍스트 추출에 OCR 기능이 사용되는지 여부를 나타내는 값입니다. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


OCR 옵션을 설정할 수 있는 기능과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | useOcr | boolean | 텍스트 추출에 OCR 기능이 사용되는지 여부를 나타내는 값입니다. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 기능에 대한 추가 옵션입니다. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


정규식을 사용하여 새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다. 다른 옵션은 기본값으로 설정됩니다(자세한 내용은 주석을 참조하십시오).

다음 속성은 기본값을 가집니다:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


정규식과 사각형 영역을 사용하여 새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다. 다른 옵션은 기본값으로 설정됩니다(자세한 내용은 주석을 참조하십시오).

다음 속성은 기본값을 가집니다:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 페이지 영역을 포함하는 사각형 영역입니다. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


정규식, 사각형 영역 및 무시된 테두리 크기를 사용하여 새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다. 다른 옵션은 기본값으로 설정됩니다(자세한 내용은 주석을 참조하십시오).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 페이지 영역을 포함하는 사각형 영역입니다. |
|
|  | rectangleTolerance | double | 사각형 영역에 의해 캡처될 때 무시되는 테두리 크기입니다. 텍스트 항목 높이의 비율로 측정됩니다. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | uniteSegments | boolean | 세그먼트가 결합되는지 여부를 나타내는 값입니다. |
|
|  | ignoreFormatting | boolean | 텍스트 서식이 무시되는지 여부를 나타내는 값입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 페이지 영역을 포함하는 사각형 영역입니다. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


무시된 테두리 크기를 지정하여 새로운 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | expression | java.lang.String | 정규식. |
|
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | uniteSegments | boolean | 세그먼트가 결합되는지 여부를 나타내는 값입니다. |
|
|  | ignoreFormatting | boolean | 텍스트 서식이 무시되는지 여부를 나타내는 값입니다. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 페이지 영역을 포함하는 사각형 영역입니다. |
|
|  | rectangleTolerance | double | 사각형 영역에 의해 캡처될 때 무시되는 테두리 크기입니다. 텍스트 항목 높이의 비율로 측정됩니다. |
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

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


세그먼트가 결합되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 세그먼트가 결합되면 {code true}, 그렇지 않으면 {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


텍스트 서식이 무시되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 텍스트 서식이 무시되면 true, 그렇지 않으면 false.

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


텍스트 추출에 OCR 커넥터가 사용되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - OCR 기능이 사용되는 경우 true, 그렇지 않으면 false.

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


OCR 기능에 대한 추가 옵션을 가져옵니다.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

