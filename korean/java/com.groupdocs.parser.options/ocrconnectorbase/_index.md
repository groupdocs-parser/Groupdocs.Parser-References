---
title: "OcrConnectorBase"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "OCR 기능을 제공합니다."
type: docs
weight: 25
url: /ko/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

OCR 기능을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | 새로운 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | 텍스트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | 텍스트 영역 추출이 지원되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | imageStream 스트림에서 텍스트를 인식합니다. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | imageStream 스트림에서 텍스트 영역을 인식합니다. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


새로운 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 클래스 인스턴스를 초기화합니다.


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


텍스트 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 텍스트 추출이 지원되는 경우 true; 그렇지 않으면 false.

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


텍스트 영역 추출이 지원되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 텍스트 추출 영역이 지원되는 경우 true; 그렇지 않으면 false.

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


imageStream 스트림에서 텍스트를 인식합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 문서 페이지의 이미지 표현입니다. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 옵션입니다. |
|

**Returns:**
java.lang.String - 인식된 텍스트를 나타내는 문자열; 텍스트 인식이 지원되지 않는 경우 null.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


imageStream 스트림에서 텍스트 영역을 인식합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 문서 페이지의 이미지 표현입니다. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | 문서 페이지의 크기입니다. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 옵션입니다. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 객체의 컬렉션; 텍스트 영역 인식이 지원되지 않는 경우 null.

