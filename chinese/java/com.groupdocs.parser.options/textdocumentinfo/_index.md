---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文本文档信息。"
type: docs
weight: 36
url: /zh/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

表示文本文档信息。

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCharset()](#getCharset--) | 获取文本文档的检测到的编码。 |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


获取文本文档的检测到的编码。


**Returns:**
java.nio.charset.Charset - Charset 类的实例。

