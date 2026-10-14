---
title: "TextOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेक्स्ट निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 37
url: /hi/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

टेक्स्ट निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

एक उदाहरण [TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का पैरामीटर के रूप में [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-) में उपयोग किया जाता है
और [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) मेथड्स। वहाँ उपयोग उदाहरण देखें।

यह टेक्स्ट निष्कर्षण के कच्चे मोड को निर्दिष्ट करने के लिए उपयोग किया जाता है। इस मोड में टेक्स्ट असटीक रूप से निकाला जाता है
तरिका लेकिन मानक मोड की तुलना में तेज़ है। यदि कच्चा मोड दस्तावेज़ फ़ॉर्मेट का समर्थन नहीं करता है,
तो यह पैरामीटर अनदेखा कर दिया जाता है और मानक मोड उपयोग किया जाता है।

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR उपयोग विकल्प के साथ आरंभ करता है। |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR विकल्प सेट करने की क्षमता के साथ आरंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | वह मान प्राप्त करता है जो दर्शाता है कि कच्चा मोड उपयोग किया गया है या नहीं। |
|
|  | [isUseOcr()](#isUseOcr--) | वह मान प्राप्त करता है जो दर्शाता है कि OCR कनेक्टर का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं। |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR कार्यक्षमता के अतिरिक्त विकल्प प्राप्त करता है। |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | वह मान प्राप्त करता है जो दर्शाता है कि निकाले गए टेक्स्ट में एनोटेशन शामिल हैं या नहीं। |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | वह मान सेट करता है जो दर्शाता है कि निकाले गए टेक्स्ट में एनोटेशन शामिल हैं या नहीं। |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | वह मान जो दर्शाता है कि कच्चा मोड उपयोग किया गया है या नहीं। |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR उपयोग विकल्प के साथ आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | वह मान जो दर्शाता है कि कच्चा मोड उपयोग किया गया है या नहीं। |
|
|  | useOcr | boolean | वह मान जो दर्शाता है कि OCR कार्यक्षमता का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं। |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) क्लास का नया उदाहरण OCR विकल्प सेट करने की क्षमता के साथ आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | वह मान जो दर्शाता है कि कच्चा मोड उपयोग किया गया है या नहीं। |
|
|  | useOcr | boolean | वह मान जो दर्शाता है कि OCR कार्यक्षमता का उपयोग टेक्स्ट निकालने के लिए किया गया है या नहीं। |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR कार्यक्षमता के अतिरिक्त विकल्प। |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


वह मान प्राप्त करता है जो दर्शाता है कि कच्चा मोड उपयोग किया गया है या नहीं।


**Returns:**
boolean -  true  यदि कच्चा मोड उपयोग किया गया है; अन्यथा,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


वह मान प्राप्त करता है जो दर्शाता है कि निकाले गए टेक्स्ट में एनोटेशन शामिल हैं या नहीं। डिफ़ॉल्ट मान है  false .


**Returns:**
boolean -  true  यदि एनोटेशन शामिल हैं; अन्यथा,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


वह मान सेट करता है जो दर्शाता है कि निकाले गए टेक्स्ट में एनोटेशन शामिल हैं या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  निकाले गए टेक्स्ट में एनोटेशन शामिल करने के लिए। |
|

