---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "फ़ाइल प्रकार पहचान की मोड को परिभाषित करता है।"
type: docs
weight: 44
url: /hi/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

फ़ाइल प्रकार पहचान की मोड को परिभाषित करता है।

## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [Default](#Default) | फ़ाइल प्रकार फ़ाइल एक्सटेंशन द्वारा पता लगाया जाता है; यदि फ़ाइल एक्सटेंशन पहचाना नहीं जाता है, तो फ़ाइल प्रकार फ़ाइल सामग्री द्वारा पता लगाया जाता है। |
|
|  | [Extension](#Extension) | फ़ाइल प्रकार केवल फ़ाइल एक्सटेंशन द्वारा पता लगाया जाता है। |
|
|  | [Content](#Content) | फ़ाइल प्रकार केवल फ़ाइल सामग्री द्वारा पता लगाया जाता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


फ़ाइल प्रकार फ़ाइल एक्सटेंशन द्वारा पता लगाया जाता है; यदि फ़ाइल एक्सटेंशन पहचाना नहीं जाता है, तो फ़ाइल प्रकार फ़ाइल सामग्री द्वारा पता लगाया जाता है।


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


फ़ाइल प्रकार केवल फ़ाइल एक्सटेंशन द्वारा पता लगाया जाता है।


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


फ़ाइल प्रकार केवल फ़ाइल सामग्री द्वारा पता लगाया जाता है।


### values() {#values--}
```
public static FileTypeDetectionMode[] values()
```




**Returns:**
com.groupdocs.parser.options.FileTypeDetectionMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileTypeDetectionMode valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)
