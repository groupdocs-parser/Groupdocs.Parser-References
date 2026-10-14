---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेक्स्ट डॉक्यूमेंट जानकारी को दर्शाता है।"
type: docs
weight: 36
url: /hi/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

टेक्स्ट डॉक्यूमेंट जानकारी को दर्शाता है।

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getCharset()](#getCharset--) | टेक्स्ट दस्तावेज़ की पहचानी गई एन्कोडिंग प्राप्त करता है। |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


टेक्स्ट दस्तावेज़ की पहचानी गई एन्कोडिंग प्राप्त करता है।


**Returns:**
java.nio.charset.Charset - एक Charset क्लास का उदाहरण।

