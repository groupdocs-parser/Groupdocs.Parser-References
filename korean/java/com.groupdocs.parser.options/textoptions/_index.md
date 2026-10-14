---
title: "TextOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 37
url: /ko/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

텍스트 추출에 사용되는 옵션을 제공합니다.

텍스트 옵션 클래스의 인스턴스인 [TextOptions](../../com.groupdocs.parser.options/textoptions) 가 [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-) 메서드의 매개변수로 사용됩니다.
그리고 [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) 메서드도 있습니다. 해당 사용 예제를 확인하십시오.

텍스트 추출의 원시 모드를 지정하는 데 사용됩니다. 이 모드의 텍스트는 정확하지 않게 추출됩니다
하지만 표준 모드보다 빠릅니다. 원시 모드가 문서 형식을 지원하지 않는 경우,
이 경우 이 매개변수는 무시되고 표준 모드가 사용됩니다.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | OCR 사용 옵션과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | OCR 옵션을 설정할 수 있는 기능과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | 원시 모드가 사용되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isUseOcr()](#isUseOcr--) | 텍스트 추출에 OCR 커넥터가 사용되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR 기능에 대한 추가 옵션을 가져옵니다. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | 추출된 텍스트에 주석이 포함되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | 추출된 텍스트에 주석이 포함되는지 여부를 나타내는 값을 설정합니다. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 원시 모드가 사용되는지 여부를 나타내는 값입니다. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


OCR 사용 옵션과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 원시 모드가 사용되는지 여부를 나타내는 값입니다. |
|
|  | useOcr | boolean | 텍스트 추출에 OCR 기능이 사용되는지 여부를 나타내는 값입니다. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


OCR 옵션을 설정할 수 있는 기능과 함께 [TextOptions](../../com.groupdocs.parser.options/textoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 원시 모드가 사용되는지 여부를 나타내는 값입니다. |
|
|  | useOcr | boolean | 텍스트 추출에 OCR 기능이 사용되는지 여부를 나타내는 값입니다. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 기능에 대한 추가 옵션입니다. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


원시 모드가 사용되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 원시 모드가 사용되는 경우 true, 그렇지 않으면 false.

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


추출된 텍스트에 주석이 포함되는지 여부를 나타내는 값을 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 주석이 포함되는 경우 true, 그렇지 않으면 false.

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


추출된 텍스트에 주석이 포함되는지 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | includeAnnotations | boolean | true - 추출된 텍스트에 주석을 포함합니다. |
|

