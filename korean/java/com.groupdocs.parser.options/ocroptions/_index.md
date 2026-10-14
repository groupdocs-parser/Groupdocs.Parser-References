---
title: "OcrOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "OCR 커넥터에 사용되는 옵션을 제공합니다."
type: docs
weight: 27
url: /ko/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

OCR 커넥터에 사용되는 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | 기본값으로 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | 직사각형 영역으로 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | 페이지 미리보기 옵션으로 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 객체와 함께 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다. |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | 직사각형 영역 및 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 객체와 함께 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다. |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 텍스트 인식을 위해 사용되는 페이지 영역을 제한하는 직사각형 영역을 가져옵니다. |
|
|  | [getHandler()](#getHandler--) | OCR 이벤트를 포착하기 위한 이벤트 핸들러를 가져옵니다. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | 맞춤법 검사기의 사용 여부를 나타내는 값을 가져옵니다. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | OCR 엔진에 전달되는 페이지를 렌더링하는 데 사용되는 페이지 미리보기 옵션을 가져옵니다. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | OCR 엔진에 전달되는 페이지를 렌더링하는 데 사용되는 페이지 미리보기 옵션을 설정합니다. |
|
|  | [getLanguage()](#getLanguage--) | 광학 문자 인식을 위해 사용되는 언어를 가져옵니다. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | 광학 문자 인식을 위해 사용되는 언어를 설정합니다. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | 텍스트 인식에 사용되는 페이지 영역을 제한하는 사각형 영역을 설정합니다. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | OCR 이벤트를 포착하기 위한 이벤트 핸들러를 설정합니다. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | 맞춤법 검사기의 사용 여부를 나타내는 값을 설정합니다. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


기본값으로 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


직사각형 영역으로 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 텍스트 인식에 사용되는 페이지 영역을 제한하는 사각형 영역. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


페이지 미리보기 옵션으로 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | OCR 엔진에 전달되는 페이지 미리보기를 렌더링하는 데 사용되는 옵션. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 객체와 함께 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR 이벤트를 포착하기 위한 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 인스턴스. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


직사각형 영역 및 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 객체와 함께 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 텍스트 인식에 사용되는 페이지 영역을 제한하는 사각형 영역. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR 이벤트를 포착하기 위한 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 인스턴스. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


[OcrOptions](../../com.groupdocs.parser.options/ocroptions) 클래스를 새 인스턴스로 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 텍스트 인식에 사용되는 페이지 영역을 제한하는 사각형 영역. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR 이벤트를 포착하기 위한 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 인스턴스. |
|
|  | useSpellCheker | boolean | 맞춤법 검사기의 사용 여부를 나타내는 값. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


텍스트 인식을 위해 사용되는 페이지 영역을 제한하는 직사각형 영역을 가져옵니다.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


OCR 이벤트를 포착하기 위한 이벤트 핸들러를 가져옵니다.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


맞춤법 검사기의 사용 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 맞춤법 검사기가 사용되는 경우 true; 그렇지 않은 경우 false.

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


OCR 엔진에 전달되는 페이지를 렌더링하는 데 사용되는 페이지 미리보기 옵션을 가져옵니다.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


OCR 엔진에 전달되는 페이지를 렌더링하는 데 사용되는 페이지 미리보기 옵션을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | 페이지 미리보기 옵션. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


광학 문자 인식을 위해 사용되는 언어를 가져옵니다.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


광학 문자 인식을 위해 사용되는 언어를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | 해당 [Language](../../com.groupdocs.parser.options/language) 열거형 값. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


텍스트 인식에 사용되는 페이지 영역을 제한하는 사각형 영역을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 전체 페이지를 스캔하기 위한 사각형, 또는 null. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


OCR 이벤트를 포착하기 위한 이벤트 핸들러를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | 이벤트 핸들러. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


맞춤법 검사기의 사용 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | useSpellChecker | boolean | 맞춤법 검사를 활성화하려면 true. |
|

