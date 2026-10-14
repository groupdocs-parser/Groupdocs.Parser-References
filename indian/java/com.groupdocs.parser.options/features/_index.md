---
title: "विशेषताएँ"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "समर्थित फीचर्स की सूची को दर्शाता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

समर्थित फ़ीचर सूची का प्रतिनिधित्व करता है। दस्तावेज़ के लिए कौन से फ़ीचर समर्थित हैं या नहीं, इसकी जानकारी प्राप्त करने की अनुमति देता है।

इस क्लास का एक उदाहरण [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) प्रॉपर्टी के रूप में उपयोग किया जाता है। वहाँ उपयोग के उदाहरण देखें।

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Features()](#Features--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | वह मान लौटाता है जो दर्शाता है कि फ़ीचर समर्थित है या नहीं। |
|
|  | [isText()](#isText--) | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट निष्कर्षण समर्थित है या नहीं। |
|
|  | [isTextPage()](#isTextPage--) | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट पेज निष्कर्षण समर्थित है या नहीं। |
|
|  | [isFormattedText()](#isFormattedText--) | वह मान प्राप्त करता है जो दर्शाता है कि स्वरूपित टेक्स्ट निष्कर्षण समर्थित है या नहीं। |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | वह मान प्राप्त करता है जो दर्शाता है कि स्वरूपित टेक्स्ट पेज निष्कर्षण समर्थित है या नहीं। |
|
|  | [isSearch()](#isSearch--) | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट खोज समर्थित है या नहीं। |
|
|  | [isHighlight()](#isHighlight--) | वह मान प्राप्त करता है जो दर्शाता है कि हाइलाइट निष्कर्षण समर्थित है या नहीं। |
|
|  | [isBarcodes()](#isBarcodes--) | वह मान प्राप्त करता है जो दर्शाता है कि बारकोड निष्कर्षण समर्थित है या नहीं। |
|
|  | [isToc()](#isToc--) | वह मान प्राप्त करता है जो दर्शाता है कि सामग्री तालिका निष्कर्षण समर्थित है या नहीं। |
|
|  | [isMetadata()](#isMetadata--) | वह मान प्राप्त करता है जो दर्शाता है कि मेटाडाटा निष्कर्षण समर्थित है या नहीं। |
|
|  | [isContainer()](#isContainer--) | वह मान प्राप्त करता है जो दर्शाता है कि कंटेनर निष्कर्षण समर्थित है या नहीं। |
|
|  | [isTextAreas()](#isTextAreas--) | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट एरिया निष्कर्षण समर्थित है या नहीं। |
|
|  | [isStructure()](#isStructure--) | वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट संरचना निष्कर्षण समर्थित है या नहीं। |
|
|  | [isImages()](#isImages--) | वह मान प्राप्त करता है जो दर्शाता है कि इमेजेज़ निष्कर्षण समर्थित है या नहीं। |
|
|  | [isHyperlinks()](#isHyperlinks--) | वह मान प्राप्त करता है जो दर्शाता है कि हाइपरलिंक निष्कर्षण समर्थित है या नहीं। |
|
|  | [isTables()](#isTables--) | वह मान प्राप्त करता है जो दर्शाता है कि टेबल्स निष्कर्षण समर्थित है या नहीं। |
|
|  | [isAnnotations()](#isAnnotations--) | वह मान प्राप्त करता है जो दर्शाता है कि एनोटेशन निष्कर्षण समर्थित है या नहीं। |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | वह मान प्राप्त करता है जो दर्शाता है कि टेम्पलेट द्वारा पार्सिंग समर्थित है या नहीं। |
|
|  | [isParseForm()](#isParseForm--) | फ़ॉर्म पार्सिंग समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है। |
|
|  | [isPreview()](#isPreview--) | पूर्वावलोकन निर्माण समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है। |
|
|  | [isPagePreview()](#isPagePreview--) | पृष्ठ पूर्वावलोकन निर्माण समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है। |
|
|  | [isOcr()](#isOcr--) | OCR कार्यक्षमता समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है। |
|
|  | [isWorksheet()](#isWorksheet--) | वर्कशीट निष्कर्षण समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है। |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


वह मान लौटाता है जो दर्शाता है कि फ़ीचर समर्थित है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | featureName | java.lang.String | फ़ीचर का नाम। |
|

**Returns:**
बूलियन -  true  यदि फ़ीचर समर्थित है; अन्यथा,  false .

### isText() {#isText--}
```
public boolean isText()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेक्स्ट निष्कर्षण समर्थित है; अन्यथा,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट पेज निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेक्स्ट पृष्ठ निष्कर्षण समर्थित है; अन्यथा,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


वह मान प्राप्त करता है जो दर्शाता है कि स्वरूपित टेक्स्ट निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि स्वरूपित टेक्स्ट निष्कर्षण समर्थित है; अन्यथा,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


वह मान प्राप्त करता है जो दर्शाता है कि स्वरूपित टेक्स्ट पेज निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि स्वरूपित टेक्स्ट पृष्ठ समर्थित है; अन्यथा,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट खोज समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेक्स्ट खोज समर्थित है; अन्यथा,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


वह मान प्राप्त करता है जो दर्शाता है कि हाइलाइट निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि हाइलाइट निष्कर्षण समर्थित है; अन्यथा,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


वह मान प्राप्त करता है जो दर्शाता है कि बारकोड निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि बारकोड निष्कर्षण समर्थित है; अन्यथा,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


वह मान प्राप्त करता है जो दर्शाता है कि सामग्री तालिका निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि सामग्री तालिका निष्कर्षण समर्थित है; अन्यथा,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


वह मान प्राप्त करता है जो दर्शाता है कि मेटाडाटा निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि मेटाडेटा निष्कर्षण समर्थित है; अन्यथा,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


वह मान प्राप्त करता है जो दर्शाता है कि कंटेनर निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि कंटेनर निष्कर्षण समर्थित है; अन्यथा,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट एरिया निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेक्स्ट क्षेत्रों का निष्कर्षण समर्थित है; अन्यथा,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेक्स्ट संरचना निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेक्स्ट संरचना निष्कर्षण समर्थित है; अन्यथा,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


वह मान प्राप्त करता है जो दर्शाता है कि इमेजेज़ निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि छवियों का निष्कर्षण समर्थित है; अन्यथा,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


वह मान प्राप्त करता है जो दर्शाता है कि हाइपरलिंक निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि हाइपरलिंक निष्कर्षण समर्थित है; अन्यथा,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेबल्स निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि तालिकाओं का निष्कर्षण समर्थित है; अन्यथा,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


वह मान प्राप्त करता है जो दर्शाता है कि एनोटेशन निष्कर्षण समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि एनोटेशन निष्कर्षण समर्थित है; अन्यथा,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


वह मान प्राप्त करता है जो दर्शाता है कि टेम्पलेट द्वारा पार्सिंग समर्थित है या नहीं।


**Returns:**
बूलियन -  true  यदि टेम्प्लेट द्वारा पार्सिंग समर्थित है; अन्यथा,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


फ़ॉर्म पार्सिंग समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि फ़ॉर्म पार्सिंग समर्थित है; अन्यथा,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


पूर्वावलोकन निर्माण समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि प्रीव्यू जेनरेशन समर्थित है; अन्यथा,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


पृष्ठ पूर्वावलोकन निर्माण समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि पेज प्रीव्यू जेनरेशन समर्थित है; अन्यथा,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


OCR कार्यक्षमता समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि OCR कार्यक्षमता समर्थित है; अन्यथा,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


वर्कशीट निष्कर्षण समर्थित है या नहीं दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि वर्कशीट एक्सट्रैक्शन समर्थित है; अन्यथा,  false .

