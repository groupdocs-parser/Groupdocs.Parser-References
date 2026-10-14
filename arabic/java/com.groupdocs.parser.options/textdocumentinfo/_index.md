---
title: "TextDocumentInfo"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات مستند النص."
type: docs
weight: 36
url: /ar/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

يمثل معلومات مستند النص.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## البناؤات

| البناء | الوصف |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getCharset()](#getCharset--) | يحصل على الترميز المكتشف لمستند النص. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


يحصل على الترميز المكتشف لمستند النص.


**Returns:**
java.nio.charset.Charset - نسخة من فئة Charset.

