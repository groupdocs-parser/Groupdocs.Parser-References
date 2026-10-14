---
title: "TextDocumentInfo"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni del documento di testo."
type: docs
weight: 36
url: /it/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Rappresenta le informazioni del documento di testo.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCharset()](#getCharset--) | Restituisce la codifica rilevata del documento di testo. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Restituisce la codifica rilevata del documento di testo.


**Returns:**
java.nio.charset.Charset - Un'istanza della classe Charset.

