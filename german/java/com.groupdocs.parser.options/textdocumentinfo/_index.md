---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Informationen zum Textdokument dar."
type: docs
weight: 36
url: /de/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Stellt die Informationen zum Textdokument dar.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCharset()](#getCharset--) | Ermittelt die erkannte Kodierung des Textdokuments. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Ermittelt die erkannte Kodierung des Textdokuments.


**Returns:**
java.nio.charset.Charset - Eine Instanz der Klasse Charset.

