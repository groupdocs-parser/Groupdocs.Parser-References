---
title: "OcrOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "OCR कनेक्टर के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 27
url: /hi/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

OCR कनेक्टर के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | डिफ़ॉल्ट मानों के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | आयताकार क्षेत्र के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | पेज प्रीव्यू विकल्पों के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) ऑब्जेक्ट के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | आयताकार क्षेत्र और [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) ऑब्जेक्ट के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | पाठ पहचान के लिए उपयोग किए जाने वाले पेज क्षेत्र को सीमित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
|  | [getHandler()](#getHandler--) | OCR इवेंट्स को पकड़ने के लिए इवेंट हैंडलर प्राप्त करता है। |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | वह मान प्राप्त करता है जो दर्शाता है कि स्पेल चेकर उपयोग किया गया है। |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | OCR इंजन को फीड किए जाने वाले पृष्ठ को रेंडर करने के लिए उपयोग किए जाने वाले पृष्ठ पूर्वावलोकन विकल्प प्राप्त करता है। |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | OCR इंजन को फीड किए जाने वाले पृष्ठ को रेंडर करने के लिए उपयोग किए जाने वाले पृष्ठ पूर्वावलोकन विकल्प सेट करता है। |
|
|  | [getLanguage()](#getLanguage--) | ऑप्टिकल कैरेक्टर रिकग्निशन के लिए उपयोग की गई भाषा प्राप्त करता है। |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | ऑप्टिकल कैरेक्टर रिकग्निशन के लिए उपयोग की गई भाषा सेट करता है। |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | पाठ पहचान के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र को सीमित करने वाले आयताकार क्षेत्र को सेट करता है। |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | OCR इवेंट्स को पकड़ने के लिए इवेंट हैंडलर सेट करता है। |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | स्पेल चेकर उपयोग किया गया है या नहीं दर्शाने वाला मान सेट करता है। |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


डिफ़ॉल्ट मानों के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


आयताकार क्षेत्र के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पाठ पहचान के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र को सीमित करने वाला आयताकार क्षेत्र। |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


पेज प्रीव्यू विकल्पों के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | OCR इंजन को फीड किए जाने वाले पृष्ठ पूर्वावलोकन को रेंडर करने के लिए उपयोग किए गए विकल्प। |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) ऑब्जेक्ट के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR इवेंट्स को पकड़ने के लिए [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) का एक उदाहरण। |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


आयताकार क्षेत्र और [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) ऑब्जेक्ट के साथ [OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पाठ पहचान के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र को सीमित करने वाला आयताकार क्षेत्र। |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR इवेंट्स को पकड़ने के लिए [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) का एक उदाहरण। |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


[OcrOptions](../../com.groupdocs.parser.options/ocroptions) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पाठ पहचान के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र को सीमित करने वाला आयताकार क्षेत्र। |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR इवेंट्स को पकड़ने के लिए [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) का एक उदाहरण। |
|
|  | useSpellCheker | boolean | स्पेल चेकर उपयोग किया गया है या नहीं दर्शाने वाला मान। |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


पाठ पहचान के लिए उपयोग किए जाने वाले पेज क्षेत्र को सीमित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


OCR इवेंट्स को पकड़ने के लिए इवेंट हैंडलर प्राप्त करता है।


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


वह मान प्राप्त करता है जो दर्शाता है कि स्पेल चेकर उपयोग किया गया है।


**Returns:**
boolean -  true  यदि स्पेल चेकर उपयोग किया गया है; अन्यथा,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


OCR इंजन को फीड किए जाने वाले पृष्ठ को रेंडर करने के लिए उपयोग किए जाने वाले पृष्ठ पूर्वावलोकन विकल्प प्राप्त करता है।


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


OCR इंजन को फीड किए जाने वाले पृष्ठ को रेंडर करने के लिए उपयोग किए जाने वाले पृष्ठ पूर्वावलोकन विकल्प सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | पृष्ठ पूर्वावलोकन विकल्प। |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


ऑप्टिकल कैरेक्टर रिकग्निशन के लिए उपयोग की गई भाषा प्राप्त करता है।


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


ऑप्टिकल कैरेक्टर रिकग्निशन के लिए उपयोग की गई भाषा सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | यह [Language](../../com.groupdocs.parser.options/language) enum मान। |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


पाठ पहचान के लिए उपयोग किए जाने वाले पृष्ठ क्षेत्र को सीमित करने वाले आयताकार क्षेत्र को सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पूरा पृष्ठ स्कैन करने के लिए आयत, या  null . |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


OCR इवेंट्स को पकड़ने के लिए इवेंट हैंडलर सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | इवेंट हैंडलर। |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


स्पेल चेकर उपयोग किया गया है या नहीं दर्शाने वाला मान सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | useSpellChecker | boolean | स्पेल जांच सक्षम करने के लिए true . |
|

