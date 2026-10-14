---
title: "FormattedTextOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "서식이 지정된 텍스트 추출에 사용되는 옵션을 제공합니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

서식이 지정된 텍스트 추출에 사용되는 옵션을 제공합니다.

인스턴스 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 클래스가 [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-) 메서드의 매개변수로 사용됩니다.
및 [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) 메서드. 해당 사용 예제를 참조하십시오.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | 모드가 설정되지 않은 새로운 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 클래스 인스턴스를 초기화합니다. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | 새로운 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getMode()](#getMode--) | 포맷된 텍스트 추출 모드를 가져옵니다. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | 포맷된 텍스트 추출 모드를 설정합니다. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


모드가 설정되지 않은 새로운 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 클래스 인스턴스를 초기화합니다.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


새로운 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | 포맷된 텍스트 추출 모드. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


포맷된 텍스트 추출 모드를 가져옵니다.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


포맷된 텍스트 추출 모드를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) 열거형은 포맷된 텍스트 추출 모드를 포함합니다. |
|

