---
title: "TextDocumentInfo"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi dokumen teks."
type: docs
weight: 36
url: /id/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Mewakili informasi dokumen teks.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCharset()](#getCharset--) | Mendapatkan enkoding yang terdeteksi dari dokumen teks. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Mendapatkan enkoding yang terdeteksi dari dokumen teks.


**Returns:**
java.nio.charset.Charset - Sebuah instance dari kelas Charset.

