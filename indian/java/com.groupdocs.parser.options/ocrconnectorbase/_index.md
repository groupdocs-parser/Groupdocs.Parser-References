---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "OCR कार्यक्षमता प्रदान करता है।"
type: docs
weight: 25
url: /hi/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

OCR कार्यक्षमता प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | एक नया उदाहरण प्रारंभ करता है [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | टेक्स्ट निष्कर्षण समर्थित है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | टेक्स्ट क्षेत्रों के निष्कर्षण का समर्थन है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | imageStream स्ट्रीम से टेक्स्ट को पहचानें। |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | imageStream स्ट्रीम से टेक्स्ट क्षेत्रों को पहचानें। |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


एक नया उदाहरण प्रारंभ करता है [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) क्लास का।


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


टेक्स्ट निष्कर्षण समर्थित है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि टेक्स्ट निष्कर्षण समर्थित है; अन्यथा,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


टेक्स्ट क्षेत्रों के निष्कर्षण का समर्थन है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि टेक्स्ट निष्कर्षण क्षेत्रों का समर्थन है; अन्यथा,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


imageStream स्ट्रीम से टेक्स्ट को पहचानें।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | दस्तावेज़ पृष्ठ की छवि प्रतिनिधित्व। |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR विकल्प। |
|

**Returns:**
java.lang.String - एक स्ट्रिंग जो पहचाने गए टेक्स्ट का प्रतिनिधित्व करती है;  null  यदि टेक्स्ट पहचान समर्थित नहीं है।

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


imageStream स्ट्रीम से टेक्स्ट क्षेत्रों को पहचानें।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | दस्तावेज़ पृष्ठ की छवि प्रतिनिधित्व। |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | दस्तावेज़ पृष्ठ का आकार। |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR विकल्प। |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स का संग्रह;  null  यदि टेक्स्ट क्षेत्रों की पहचान समर्थित नहीं है।

