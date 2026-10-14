---
title: "TextDocumentInfo"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations du document texte."
type: docs
weight: 36
url: /fr/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Représente les informations du document texte.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Constructors

| Constructor | Description |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [getCharset()](#getCharset--) | Obtient l'encodage détecté du document texte. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Obtient l'encodage détecté du document texte.


**Returns:**
java.nio.charset.Charset - Une instance de la classe  Charset .

