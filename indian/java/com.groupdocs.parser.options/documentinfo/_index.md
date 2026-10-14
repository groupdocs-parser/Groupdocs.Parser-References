---
title: "DocumentInfo"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "दस्तावेज़ जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

दस्तावेज़ जानकारी का प्रतिनिधित्व करता है।

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileType()](#getFileType--) | दस्तावेज़ प्रकार प्राप्त करता है। |
|
|  | [getPageCount()](#getPageCount--) | दस्तावेज़ पृष्ठों की कुल संख्या प्राप्त करता है। |
|
|  | [getRawPageCount()](#getRawPageCount--) | दस्तावेज़ के कच्चे पृष्ठों की कुल संख्या प्राप्त करता है। |
|
|  | [getSize()](#getSize--) | दस्तावेज़ का आकार बाइट्स में प्राप्त करता है। |
|
|  | [getPages()](#getPages--) | पृष्ठों के बारे में जानकारी प्राप्त करता है, जैसे कि अनुक्रमणिका और पृष्ठ आकार। |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


दस्तावेज़ प्रकार प्राप्त करता है।


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


दस्तावेज़ पृष्ठों की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक पूर्णांक मान जो पृष्ठों की कुल संख्या को दर्शाता है।

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


दस्तावेज़ के कच्चे पृष्ठों की कुल संख्या प्राप्त करता है।

कच्चा पाठ निष्कर्षण के लिए [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) प्रॉपर्टी का उपयोग करें, [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) प्रॉपर्टी के बजाय।
कुछ दस्तावेज़ सटीक और कच्चा पाठ निष्कर्षण मोड में अलग पृष्ठ संख्याएँ रखते हैं।
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - एक पूर्णांक मान जो कच्चे पृष्ठों की कुल संख्या को दर्शाता है।

### getSize() {#getSize--}
```
public abstract long getSize()
```


दस्तावेज़ का आकार बाइट्स में प्राप्त करता है।


**Returns:**
long - एक पूर्णांक मान जो दस्तावेज़ का आकार बाइट्स में दर्शाता है।

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


पृष्ठों के बारे में जानकारी प्राप्त करता है, जैसे कि अनुक्रमणिका और पृष्ठ आकार।


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - [PageInfo](../../com.groupdocs.parser.options/pageinfo) क्लासों के उदाहरणों का संग्रह।

