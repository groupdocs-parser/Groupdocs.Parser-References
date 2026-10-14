---
title: "기능"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "지원되는 기능 목록을 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

지원되는 기능 목록을 나타냅니다. 문서에 대해 어떤 기능이 지원되는지 여부에 대한 정보를 얻을 수 있습니다.

이 클래스의 인스턴스는 [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) 속성으로 사용됩니다. 해당 사용 예제를 확인하십시오.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Features()](#Features--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | 기능이 지원되는지 여부를 나타내는 값을 반환합니다. |
|
|  | [isText()](#isText--) | 텍스트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isTextPage()](#isTextPage--) | 텍스트 페이지 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isFormattedText()](#isFormattedText--) | 서식이 지정된 텍스트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | 서식이 지정된 텍스트 페이지 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isSearch()](#isSearch--) | 텍스트 검색이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isHighlight()](#isHighlight--) | 하이라이트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isBarcodes()](#isBarcodes--) | 바코드 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isToc()](#isToc--) | 목차 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isMetadata()](#isMetadata--) | 메타데이터 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isContainer()](#isContainer--) | 컨테이너 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isTextAreas()](#isTextAreas--) | 텍스트 영역 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isStructure()](#isStructure--) | 텍스트 구조 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isImages()](#isImages--) | 이미지 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isHyperlinks()](#isHyperlinks--) | 하이퍼링크 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isTables()](#isTables--) | 표 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isAnnotations()](#isAnnotations--) | 주석 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | 템플릿에 의한 파싱이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isParseForm()](#isParseForm--) | 양식 파싱이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isPreview()](#isPreview--) | 미리보기 생성이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isPagePreview()](#isPagePreview--) | 페이지 미리보기 생성이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isOcr()](#isOcr--) | OCR 기능이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isWorksheet()](#isWorksheet--) | 워크시트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


기능이 지원되는지 여부를 나타내는 값을 반환합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | featureName | java.lang.String | 특성 이름. |
|

**Returns:**
boolean -  true  if the feature is supported; otherwise,  false .

### isText() {#isText--}
```
public boolean isText()
```


텍스트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if text extraction is supported; otherwise,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


텍스트 페이지 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if text page extraction is supported; otherwise,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


서식이 지정된 텍스트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if formatted text extraction is supported; otherwise,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


서식이 지정된 텍스트 페이지 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if formatted text page is supported; otherwise,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


텍스트 검색이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 텍스트 검색이 지원되는 경우; 그렇지 않으면,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


하이라이트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 하이라이트 추출이 지원되는 경우; 그렇지 않으면,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


바코드 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 바코드 추출이 지원되는 경우; 그렇지 않으면,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


목차 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 목차 추출이 지원되는 경우; 그렇지 않으면,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


메타데이터 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 메타데이터 추출이 지원되는 경우; 그렇지 않으면,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


컨테이너 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 컨테이너 추출이 지원되는 경우; 그렇지 않으면,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


텍스트 영역 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 텍스트 영역 추출이 지원되는 경우; 그렇지 않으면,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


텍스트 구조 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 텍스트 구조 추출이 지원되는 경우; 그렇지 않으면,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


이미지 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 이미지 추출이 지원되는 경우; 그렇지 않으면,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


하이퍼링크 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 하이퍼링크 추출이 지원되는 경우; 그렇지 않으면,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


표 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 테이블 추출이 지원되는 경우; 그렇지 않으면,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


주석 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 주석 추출이 지원되는 경우; 그렇지 않으면,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


템플릿에 의한 파싱이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 템플릿 기반 파싱이 지원되는 경우; 그렇지 않으면,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


양식 파싱이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 양식 파싱이 지원되는 경우; 그렇지 않으면,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


미리보기 생성이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 미리보기 생성이 지원되는 경우; 그렇지 않으면,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


페이지 미리보기 생성이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 페이지 미리보기 생성이 지원되는 경우; 그렇지 않으면,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


OCR 기능이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if OCR 기능이 지원되는 경우; 그렇지 않으면,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


워크시트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  if 워크시트 추출이 지원되는 경우; 그렇지 않으면,  false .

