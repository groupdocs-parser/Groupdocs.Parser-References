---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "पेज टेक्स्ट एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 32
url: /hi/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

पेज टेक्स्ट एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

एक उदाहरण [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का पैरामीटर के रूप में उपयोग किया जाता है [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
और [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) मेथड्स। वहाँ उपयोग उदाहरण देखें।

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | डिफ़ॉल्ट मानों के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR उपयोग विकल्प के साथ आरंभ करता है। |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR विकल्प सेट करने की क्षमता के साथ आरंभ करता है। |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | नियमित अभिव्यक्ति के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | नियमित अभिव्यक्ति और आयताकार क्षेत्र के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | नियमित अभिव्यक्ति, आयताकार क्षेत्र और अनदेखी सीमा के आकार के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | अनदेखी सीमा के आकार के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getExpression()](#getExpression--) | नियमित अभिव्यक्ति प्राप्त करता है। |
|
|  | [isMatchCase()](#isMatchCase--) | उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | [isUniteSegments()](#isUniteSegments--) | उस मान को प्राप्त करता है जो दर्शाता है कि खंड एकीकृत हैं। |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट फ़ॉर्मेटिंग को अनदेखा किया गया है। |
|
|  | [isUseOcr()](#isUseOcr--) | वह मान प्राप्त करता है जो दर्शाता है कि OCR कनेक्टर का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं। |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR कार्यक्षमता के अतिरिक्त विकल्प प्राप्त करता है। |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


डिफ़ॉल्ट मानों के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है।


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR उपयोग विकल्प के साथ आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | useOcr | boolean | वह मान जो दर्शाता है कि OCR कार्यक्षमता का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं। |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR विकल्प सेट करने की क्षमता के साथ आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | useOcr | boolean | वह मान जो दर्शाता है कि OCR कार्यक्षमता का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं। |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR कार्यक्षमता के अतिरिक्त विकल्प। |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


नियमित अभिव्यक्ति के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)।

निम्नलिखित प्रॉपर्टीज़ के डिफ़ॉल्ट मान हैं:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


नियमित अभिव्यक्ति और आयताकार क्षेत्र के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)।

निम्नलिखित प्रॉपर्टीज़ के डिफ़ॉल्ट मान हैं:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ क्षेत्रों को सम्मिलित करने वाला आयताकार क्षेत्र। |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


नियमित अभिव्यक्ति, आयताकार क्षेत्र और अनदेखी सीमा के आकार के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ क्षेत्रों को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | rectangleTolerance | double | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार। इसे टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


[PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | uniteSegments | boolean | वह मान जो दर्शाता है कि क्या खंड एकीकृत किए गए हैं। |
|
|  | ignoreFormatting | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट फ़ॉर्मेटिंग को अनदेखा किया गया है। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ क्षेत्रों को सम्मिलित करने वाला आयताकार क्षेत्र। |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


अनदेखी सीमा के आकार के साथ [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | expression | java.lang.String | नियमित अभिव्यक्ति। |
|
|  | matchCase | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट केस को अनदेखा नहीं किया गया है। |
|
|  | uniteSegments | boolean | वह मान जो दर्शाता है कि क्या खंड एकीकृत किए गए हैं। |
|
|  | ignoreFormatting | boolean | वह मान जो दर्शाता है कि क्या टेक्स्ट फ़ॉर्मेटिंग को अनदेखा किया गया है। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ क्षेत्रों को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | rectangleTolerance | double | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखी की जाने वाली सीमा का आकार। इसे टेक्स्ट आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


नियमित अभिव्यक्ति प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जो नियमित अभिव्यक्ति को दर्शाती है।

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट केस को अनदेखा नहीं किया गया है।


**Returns:**
boolean -  true  यदि टेक्स्ट केस को अनदेखा नहीं किया गया है; अन्यथा,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


उस मान को प्राप्त करता है जो दर्शाता है कि खंड एकीकृत हैं।


**Returns:**
boolean - {code true} यदि खंड एकीकृत किए गए हैं; अन्यथा, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


उस मान को प्राप्त करता है जो दर्शाता है कि टेक्स्ट फ़ॉर्मेटिंग को अनदेखा किया गया है।


**Returns:**
boolean -  true  यदि टेक्स्ट फ़ॉर्मेटिंग को अनदेखा किया गया है; अन्यथा,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


वह मान प्राप्त करता है जो दर्शाता है कि OCR कनेक्टर का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं।


**Returns:**
boolean -  true  यदि OCR कार्यक्षमता उपयोग की गई है; अन्यथा,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


OCR कार्यक्षमता के अतिरिक्त विकल्प प्राप्त करता है।


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

