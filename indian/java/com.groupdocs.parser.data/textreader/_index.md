---
title: "TextReader"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "एक रीडर का प्रतिनिधित्व करता है जो क्रमिक अक्षरों की श्रृंखला पढ़ सकता है।"
type: docs
weight: 29
url: /hi/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

एक रीडर का प्रतिनिधित्व करता है जो क्रमिक अक्षरों की श्रृंखला पढ़ सकता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | टेक्स्ट रीडर से अक्षरों की एक पंक्ति पढ़ता है और डेटा को स्ट्रिंग के रूप में लौटाता है। |
|
|  | [readToEnd()](#readToEnd--) | वर्तमान स्थिति से टेक्स्ट रीडर के अंत तक सभी अक्षर पढ़ता है और उन्हें एक स्ट्रिंग के रूप में लौटाता है। |
|
|  | [dispose()](#dispose--) | [TextReader](../../com.groupdocs.parser.data/textreader) ऑब्जेक्ट द्वारा उपयोग किए गए सभी संसाधनों को रिलीज़ करता है। |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


टेक्स्ट रीडर से अक्षरों की एक पंक्ति पढ़ता है और डेटा को स्ट्रिंग के रूप में लौटाता है।


**Returns:**
java.lang.String - रीडर से अगली पंक्ति, या यदि सभी अक्षर पढ़ लिए गए हों तो  null  ।

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


वर्तमान स्थिति से टेक्स्ट रीडर के अंत तक सभी अक्षर पढ़ता है और उन्हें एक स्ट्रिंग के रूप में लौटाता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जिसमें वर्तमान स्थिति से टेक्स्ट रीडर के अंत तक के सभी अक्षर होते हैं।

### dispose() {#dispose--}
```
public void dispose()
```


[TextReader](../../com.groupdocs.parser.data/textreader) ऑब्जेक्ट द्वारा उपयोग किए गए सभी संसाधनों को रिलीज़ करता है।


