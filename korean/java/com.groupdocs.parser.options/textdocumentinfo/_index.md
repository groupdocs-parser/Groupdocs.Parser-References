---
title: "TextDocumentInfo"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트 문서 정보를 나타냅니다."
type: docs
weight: 36
url: /ko/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

텍스트 문서 정보를 나타냅니다.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCharset()](#getCharset--) | 텍스트 문서의 감지된 인코딩을 가져옵니다. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


텍스트 문서의 감지된 인코딩을 가져옵니다.


**Returns:**
java.nio.charset.Charset - Charset 클래스의 인스턴스입니다.

