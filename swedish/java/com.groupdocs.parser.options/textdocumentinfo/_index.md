---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar informationen om textdokumentet."
type: docs
weight: 36
url: /sv/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Representerar informationen om textdokumentet.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCharset()](#getCharset--) | Hämtar den upptäckta kodningen av textdokumentet. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Hämtar den upptäckta kodningen av textdokumentet.


**Returns:**
java.nio.charset.Charset - En instans av  Charset  klass.

