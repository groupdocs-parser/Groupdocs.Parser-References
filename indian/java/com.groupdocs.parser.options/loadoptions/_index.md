---
title: "LoadOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "फ़ाइल खोलने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

फ़ाइल खोलने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

इस क्लास का एक उदाहरण [Parser](../../com.groupdocs.parser/parser) क्लास के कंस्ट्रक्टर्स में पैरामीटर के रूप में उपयोग किया जाता है:

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

वहाँ उपयोग उदाहरण देखें।

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण टाइमआउट के साथ प्रारंभ करता है। |
|
|  | [LoadOptions()](#LoadOptions--) | खाली Password, FileFormat को FileFormat.Unknown के बराबर और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | FileFormat को FileFormat.Unknown के बराबर और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | खाली Password और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | कस्टम एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | पूरी तरह कस्टमाइज़्ड क्लास के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | खाली Password और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | पासवर्ड और डिफ़ॉल्ट एन्कोडिंग्स के साथ [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | कस्टम एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | पूरी तरह कस्टमाइज़्ड क्लास के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | फ़ाइल फ़ॉर्मेट प्राप्त करता है। |
|
|  | [getFileType()](#getFileType--) | फ़ाइल प्रकार प्राप्त करता है। |
|
|  | [getPassword()](#getPassword--) | पासवर्ड प्राप्त करता है। |
|
|  | [getCharset()](#getCharset--) | दस्तावेज़ की एन्कोडिंग प्राप्त करता है। |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | डिफ़ॉल्ट ANSI एन्कोडिंग प्राप्त करता है जो एन्कोडिंग पहचान के लिए उपयोग की जाती है। |
|
|  | [getTimeout()](#getTimeout--) | वह मान प्राप्त करता है जो प्रतीक्षा करने के मिलीसेकंड की संख्या को दर्शाता है। |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण टाइमआउट के साथ प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | टाइमआउट | java.time.Duration | वह Duration जो प्रतीक्षा करने के मिलीसेकंड की संख्या को दर्शाता है। |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


खाली Password, FileFormat को FileFormat.Unknown के बराबर और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


FileFormat को FileFormat.Unknown के बराबर और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


खाली Password और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | फ़ाइल का फ़ॉर्मेट। |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | फ़ाइल का फ़ॉर्मेट। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


कस्टम एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | फ़ाइल का फ़ॉर्मेट। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|
|  | charset | java.nio.charset.Charset | दस्तावेज़ की एन्कोडिंग। |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग पहचान के लिए उपयोग की जाती है। |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


पूरी तरह कस्टमाइज़्ड क्लास के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | फ़ाइल का फ़ॉर्मेट। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|
|  | charset | java.nio.charset.Charset | दस्तावेज़ की एन्कोडिंग। |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग पहचान के लिए उपयोग की जाती है। |
|
|  | टाइमआउट | java.time.Duration | वह Duration जो प्रतीक्षा करने के मिलीसेकंड की संख्या को दर्शाता है। |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


खाली Password और डिफ़ॉल्ट एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | फ़ाइल का प्रकार। |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


पासवर्ड और डिफ़ॉल्ट एन्कोडिंग्स के साथ [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | फ़ाइल का प्रकार। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


कस्टम एन्कोडिंग्स के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | फ़ाइल का प्रकार। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|
|  | charset | java.nio.charset.Charset | दस्तावेज़ की एन्कोडिंग। |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग पहचान के लिए उपयोग की जाती है। |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


पूरी तरह कस्टमाइज़्ड क्लास के साथ नए [LoadOptions](../../com.groupdocs.parser.options/loadoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | फ़ाइल का प्रकार। |
|
|  | पासवर्ड | java.lang.String | पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड। |
|
|  | charset | java.nio.charset.Charset | दस्तावेज़ की एन्कोडिंग। |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग पहचान के लिए उपयोग की जाती है। |
|
|  | टाइमआउट | java.time.Duration | वह Duration जो प्रतीक्षा करने के मिलीसेकंड की संख्या को दर्शाता है। |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


फ़ाइल फ़ॉर्मेट प्राप्त करता है।


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


फ़ाइल प्रकार प्राप्त करता है।


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


पासवर्ड प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो पासवर्ड-संरक्षित फ़ाइल को खोलने के लिए पासवर्ड दर्शाता है।

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


दस्तावेज़ की एन्कोडिंग प्राप्त करता है।


**Returns:**
java.nio.charset.Charset - एक Charset क्लास का उदाहरण जो दस्तावेज़ की एन्कोडिंग दर्शाता है; null यदि सेट नहीं है।

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


डिफ़ॉल्ट ANSI एन्कोडिंग प्राप्त करता है जो एन्कोडिंग पहचान के लिए उपयोग की जाती है।


**Returns:**
java.nio.charset.Charset - एक Charset क्लास का उदाहरण जो दस्तावेज़ की एन्कोडिंग दर्शाता है; null यदि सेट नहीं है।

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


वह मान प्राप्त करता है जो प्रतीक्षा करने के मिलीसेकंड की संख्या को दर्शाता है।


**Returns:**
java.time.Duration - एक Duration का उदाहरण जो प्रतीक्षा करने के मिलीसेकंड की संख्या को दर्शाता है।

