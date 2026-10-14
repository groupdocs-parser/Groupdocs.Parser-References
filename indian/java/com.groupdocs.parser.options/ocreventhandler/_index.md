---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "OCR इवेंट्स के लिए हैंडलर प्रदान करता है।"
type: docs
weight: 26
url: /hi/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

OCR इवेंट्स के लिए हैंडलर प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | नए [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | चेतावनी संदेशों की सूची प्राप्त करता है। |
|
|  | [hasWarnings()](#hasWarnings--) | वह मान प्राप्त करता है जो दर्शाता है कि चेतावनियों की सूची खाली नहीं है। |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | पृष्ठ के साथ  pageIndex के लिए चेतावनी संदेशों की सूची लौटाता है। |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | पृष्ठ के लिए चेतावनी संदेश सेट करता है। |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


नए [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) क्लास का एक नया उदाहरण प्रारंभ करता है।


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


चेतावनी संदेशों की सूची प्राप्त करता है।


**Returns:**
java.util.List<java.lang.String> - सभी पृष्ठों के लिए चेतावनी संदेशों की सूची।

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


वह मान प्राप्त करता है जो दर्शाता है कि चेतावनियों की सूची खाली नहीं है।


**Returns:**
boolean -  true  यदि चेतावनी सूची खाली नहीं है; अन्यथा,  false ।

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


पृष्ठ के साथ  pageIndex के लिए चेतावनी संदेशों की सूची लौटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|

**Returns:**
java.util.List<java.lang.String> - पृष्ठ के लिए चेतावनी संदेशों की सूची; यदि पृष्ठ के लिए कोई चेतावनी संदेश नहीं है तो खाली सूची।

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


पृष्ठ के लिए चेतावनी संदेश सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | शून्य-आधारित पृष्ठ सूचकांक। |
|
|  | चेतावनियाँ | java.lang.Iterable<java.lang.String> | पृष्ठ के लिए चेतावनी संदेशों की सूची। |
|

