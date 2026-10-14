---
title: "TextDocumentInfo"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la información del documento de texto."
type: docs
weight: 36
url: /es/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Representa la información del documento de texto.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCharset()](#getCharset--) | Obtiene la codificación detectada del documento de texto. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Obtiene la codificación detectada del documento de texto.


**Returns:**
java.nio.charset.Charset - Una instancia de la clase Charset.

