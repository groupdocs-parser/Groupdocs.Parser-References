---
title: "HighlightOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "검색 시나리오에서 찾은 텍스트 주변의 텍스트 블록을 강조 표시하는 데 사용되는 옵션을 제공합니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

검색 시나리오에서 찾은 텍스트 주변의 텍스트 블록(하이라이트)을 추출하는 데 사용되는 옵션을 제공합니다.

다음 메서드인 [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-)에서 매개변수로 사용되는 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스의 인스턴스입니다.
그곳의 사용 예제를 확인하십시오.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | 제한이 설정되지 않은 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | 고정 길이 강조 표시를 추출하는 데 사용되는 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | 라인 제한 강조 표시를 추출하는 데 사용되는 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | 고정 단어 수 강조 표시를 추출하는 데 사용되는 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | 최대 텍스트 길이를 가져옵니다. |
|
|  | [getWordCount()](#getWordCount--) | 최대 단어 수를 가져옵니다. |
|
|  | [isLineLimited()](#isLineLimited--) | 강조 표시 추출이 텍스트 라인의 시작(또는 끝)으로 제한되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | 최대 텍스트 길이를 설정합니다. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | 최대 단어 수를 설정합니다. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | 강조 표시 추출이 텍스트 라인의 시작(또는 끝)으로 제한되는지 여부를 나타내는 값을 설정합니다. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


제한이 설정되지 않은 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다. 파서에 전달하기 전에 #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) 중 최소 하나를 설정하십시오.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


고정 길이 강조 표시를 추출하는 데 사용되는 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | maxLength | int | 최대 텍스트 길이. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


라인 제한 강조 표시를 추출하는 데 사용되는 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 최대 텍스트 길이. |
|
|  | isLineLimited | boolean | 텍스트 라인의 시작(또는 끝)으로 강조 추출이 제한되는지를 나타내는 값입니다. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


고정 단어 수 강조 표시를 추출하는 데 사용되는 새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 최대 텍스트 길이. |
|
|  | wordCount | int | 최대 단어 수입니다. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


새로운 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 최대 텍스트 길이. |
|
|  | wordCount | java.lang.Integer | 최대 단어 수입니다. |
|
|  | isLineLimited | boolean | 텍스트 라인의 시작(또는 끝)으로 강조 추출이 제한되는지를 나타내는 값입니다. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


최대 텍스트 길이를 가져옵니다.


**Returns:**
java.lang.Integer - 최대 텍스트 길이를 나타내는 양의 정수 값;  null  텍스트 길이가 제한되지 않은 경우.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


최대 단어 수를 가져옵니다.


**Returns:**
java.lang.Integer - 최대 단어 수를 나타내는 양의 정수 값;  null  단어 수가 제한되지 않은 경우.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


강조 표시 추출이 텍스트 라인의 시작(또는 끝)으로 제한되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  텍스트 라인의 시작(또는 끝)으로 강조 추출이 제한되는 경우; 그렇지 않으면  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


최대 텍스트 길이를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 음수가 아닌 정수;  null  길이 제한을 제거하려면. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


최대 단어 수를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | 음수가 아닌 정수;  null  단어 수 제한을 제거하려면. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


강조 표시 추출이 텍스트 라인의 시작(또는 끝)으로 제한되는지 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | lineLimited | boolean | true  라인 경계로 제한하려면. |
|

