---
title: TextDocumentInfo
second_title: GroupDocs.Parser for Java API Reference
description: Represents the text document information.
type: docs
weight: 33
url: /java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Represents the text document information.

**Learn more:**

 *  [Get document info][]
 *  [Detect encoding][]


[Get document info]: https://docs.groupdocs.com/display/parserjava/Get+document+info
[Detect encoding]: https://docs.groupdocs.com/display/parserjava/Detect+encoding
## Constructors

| Constructor | Description |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getCharset()](#getCharset--) | Gets the detected encoding of the text document. |
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Gets the detected encoding of the text document.

**Returns:**
java.nio.charset.Charset - An instance of  Charset  class.
