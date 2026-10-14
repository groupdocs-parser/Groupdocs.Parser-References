---
title: "FileInfo"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "फ़ाइल जानकारी को दर्शाता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

फ़ाइल जानकारी को दर्शाता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileType()](#getFileType--) | दस्तावेज़ प्रकार प्राप्त करता है। |
|
|  | [getSize()](#getSize--) | दस्तावेज़ का आकार बाइट्स में प्राप्त करता है। |
|
|  | [isEncrypted()](#isEncrypted--) | एक मान प्राप्त करता है जो दर्शाता है कि फ़ाइल पासवर्ड-संरक्षित है या नहीं। |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


दस्तावेज़ प्रकार प्राप्त करता है।


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


दस्तावेज़ का आकार बाइट्स में प्राप्त करता है।


**Returns:**
long - एक पूर्णांक मान जो दस्तावेज़ का आकार बाइट्स में दर्शाता है।

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


एक मान प्राप्त करता है जो दर्शाता है कि फ़ाइल पासवर्ड-संरक्षित है या नहीं।


**Returns:**
boolean - एक बूलियन true यदि फ़ाइल पासवर्ड-संरक्षित है; अन्यथा false.

