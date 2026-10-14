---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de informatie van het tekstdocument voor."
type: docs
weight: 36
url: /nl/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Stelt de informatie van het tekstdocument voor.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCharset()](#getCharset--) | Haalt de gedetecteerde codering van het tekstdocument op. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Haalt de gedetecteerde codering van het tekstdocument op.


**Returns:**
java.nio.charset.Charset - Een instantie van de Charset-klasse.

