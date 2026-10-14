---
title: "ContainerItem"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "Zip आर्काइव इकाई, ईमेल अटैचमेंट, PDF पोर्टफोलियो आइटम आदि जैसी कंटेनर आइटम का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

एक कंटेनर आइटम का प्रतिनिधित्व करता है जैसे ज़िप आर्काइव एंटिटी, ईमेल अटैचमेंट, पीडीएफ पोर्टफोलियो आइटम आदि।

[ContainerItem](../../com.groupdocs.parser.data/containeritem) क्लास का एक उदाहरण [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) मेथड के रिटर्न वैल्यू के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | [ContainerItem](../../com.groupdocs.parser.data/containeritem) का नया उदाहरण आइटम के नाम और डायरेक्टरी के साथ इनिशियलाइज़ करता है। |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | [ContainerItem](../../com.groupdocs.parser.data/containeritem) का नया उदाहरण आइटम के पूर्ण पाथ के साथ इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getName()](#getName--) | आइटम का नाम प्राप्त करता है। |
|
|  | [getDirectory()](#getDirectory--) | आइटम की डायरेक्टरी प्राप्त करता है। |
|
|  | [getFilePath()](#getFilePath--) | आइटम का पूर्ण पाथ प्राप्त करता है। |
|
|  | [getSize()](#getSize--) | आइटम का आकार प्राप्त करता है। |
|
|  | [getMetadata()](#getMetadata--) | मेटाडाटा आइटम्स का संग्रह प्राप्त करता है। |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | मेटाडाटा मान प्राप्त करता है। |
|
|  | [openStream()](#openStream--) | आइटम कंटेंट की स्ट्रीम खोलता है। |
|
|  | [openParser()](#openParser--) | आइटम कंटेंट के लिए [Parser](../../com.groupdocs.parser/parser) ऑब्जेक्ट बनाता है। |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) के साथ आइटम कंटेंट के लिए [Parser](../../com.groupdocs.parser/parser) ऑब्जेक्ट बनाता है। |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) और [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ आइटम कंटेंट के लिए [Parser](../../com.groupdocs.parser/parser) ऑब्जेक्ट बनाता है। |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | कंटेनर आइटम का फ़ाइल प्रकार पता करता है। |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


[ContainerItem](../../com.groupdocs.parser.data/containeritem) का नया उदाहरण आइटम के नाम और डायरेक्टरी के साथ इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | नाम | java.lang.String | आइटम का नाम। |
|
|  | डायरेक्टरी | java.lang.String | आइटम की डायरेक्टरी। |
|
|  | size | long | आइटम का आकार। |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | मेटाडाटा आइटम्स का संग्रह। |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


[ContainerItem](../../com.groupdocs.parser.data/containeritem) का नया उदाहरण आइटम के पूर्ण पाथ के साथ इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | आइटम का पूर्ण पाथ। |
|
|  | size | long | आइटम का आकार। |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | मेटाडाटा आइटम्स का संग्रह। |
|

### getName() {#getName--}
```
public String getName()
```


आइटम का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग वैल्यू जो आइटम की फ़ाइल नाम (डायरेक्टरी के बिना) को दर्शाती है।

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


आइटम की डायरेक्टरी प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग वैल्यू जो आइटम की डायरेक्टरी (फ़ाइल नाम के बिना) को दर्शाती है।

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


आइटम का पूर्ण पाथ प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग वैल्यू जो आइटम का पूर्ण पाथ दर्शाती है।

### getSize() {#getSize--}
```
public long getSize()
```


आइटम का आकार प्राप्त करता है।


**Returns:**
long - एक इंटेजर वैल्यू जो आइटम का आकार बाइट्स में दर्शाती है।

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


मेटाडाटा आइटम्स का संग्रह प्राप्त करता है।


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - एक संग्रह है [MetadataItem](../../com.groupdocs.parser.data/metadataitem) वस्तुओं का; यदि मेटाडेटा सेट नहीं है तो खाली।

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


मेटाडाटा मान प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | नाम | java.lang.String | मेटाडेटा का नाम। |
|

**Returns:**
java.lang.String - एक स्ट्रिंग मान जो मेटाडेटा आइटम के मान को दर्शाता है; यदि इस नाम के साथ मेटाडेटा नहीं मिलता तो  null  ।

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


आइटम कंटेंट की स्ट्रीम खोलता है।


**Returns:**
java.io.InputStream - आइटम सामग्री वाला एक स्ट्रीम।

### openParser() {#openParser--}
```
public Parser openParser()
```


आइटम कंटेंट के लिए [Parser](../../com.groupdocs.parser/parser) ऑब्जेक्ट बनाता है।


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) के साथ आइटम कंटेंट के लिए [Parser](../../com.groupdocs.parser/parser) ऑब्जेक्ट बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | आइटम सामग्री खोलने के विकल्प। |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


[LoadOptions](../../com.groupdocs.parser.options/loadoptions) और [ParserSettings](../../com.groupdocs.parser.options/parsersettings) के साथ आइटम कंटेंट के लिए [Parser](../../com.groupdocs.parser/parser) ऑब्जेक्ट बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | आइटम सामग्री खोलने के विकल्प। |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | पार्सर सेटिंग्स जो डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाती हैं। |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


कंटेनर आइटम का फ़ाइल प्रकार पता करता है।


detectionMode
पैरामीटर फ़ाइल प्रकार पहचान को नियंत्रित करने की क्षमता प्रदान करता है:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

निम्नलिखित उदाहरण दिखाता है कि कंटेनर आइटम का फ़ाइल प्रकार कैसे पता करें:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | फ़ाइल प्रकार पहचान की मोड को परिभाषित करता है। |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

