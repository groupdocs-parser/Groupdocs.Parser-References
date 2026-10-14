---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αναπαριστά τις πληροφορίες του κειμενικού εγγράφου."
type: docs
weight: 36
url: /el/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

Αναπαριστά τις πληροφορίες του κειμενικού εγγράφου.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCharset()](#getCharset--) | Λαμβάνει την ανιχνευμένη κωδικοποίηση του εγγράφου κειμένου. |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


Λαμβάνει την ανιχνευμένη κωδικοποίηση του εγγράφου κειμένου.


**Returns:**
java.nio.charset.Charset - Μία παρουσία της κλάσης Charset.

