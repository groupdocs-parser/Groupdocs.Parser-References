---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "बारकोड निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

बारकोड निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | BarcodeOptions क्लास का एक नया इंस्टेंस डिफ़ॉल्ट मानों के साथ इनिशियलाइज़ करता है। |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | BarcodeOptions क्लास का एक नया इंस्टेंस आयताकार क्षेत्र के साथ इनिशियलाइज़ करता है। |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | BarcodeOptions क्लास का एक नया इंस्टेंस गुणवत्ता सेटिंग्स और कोड प्रकारों के साथ इनिशियलाइज़ करता है। |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | BarcodeOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | वह मान प्राप्त करता है जो दर्शाता है कि क्या गलत बारकोड की अनुमति है। |
|
|  | [getDimension()](#getDimension--) | बारकोड न्यूनतम तत्व का न्यूनतम आकार प्राप्त करता है। |
|
|  | [getImageQuality()](#getImageQuality--) | स्रोत छवि की गुणवत्ता प्राप्त करता है। |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | स्रोत बारकोड की गुणवत्ता प्राप्त करता है। |
|
|  | [getRectangle()](#getRectangle--) | पृष्ठ क्षेत्रों को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है। |
|
|  | [getCodeTypes()](#getCodeTypes--) | पढ़ने के लिए बारकोड प्रकार प्राप्त करता है। |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | वह मान सेट करता है जो दर्शाता है कि क्या गलत बारकोड की अनुमति है। |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | बारकोड न्यूनतम तत्व का न्यूनतम आकार सेट करता है। |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | स्रोत छवि की गुणवत्ता सेट करता है। |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | स्रोत बारकोड की गुणवत्ता सेट करता है। |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | बारकोड वाले आयताकार क्षेत्र को सेट करता है। |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | पढ़ने के लिए बारकोड प्रकार सेट करता है। |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


BarcodeOptions क्लास का एक नया इंस्टेंस डिफ़ॉल्ट मानों के साथ इनिशियलाइज़ करता है।


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


BarcodeOptions क्लास का एक नया इंस्टेंस आयताकार क्षेत्र के साथ इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | बारकोड्स को सम्मिलित करने वाला आयताकार क्षेत्र। |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


BarcodeOptions क्लास का एक नया इंस्टेंस गुणवत्ता सेटिंग्स और कोड प्रकारों के साथ इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | स्रोत छवि की गुणवत्ता। |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | स्रोत बारकोड की गुणवत्ता। |
|
|  | codeTypes | java.lang.String[] | पढ़ने के लिए बारकोड के प्रकार। |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


BarcodeOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | बारकोड्स को सम्मिलित करने वाला आयताकार क्षेत्र। |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | स्रोत छवि की गुणवत्ता। |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | स्रोत बारकोड की गुणवत्ता। |
|
|  | dimension | java.lang.Float | बारकोड के न्यूनतम तत्व का न्यूनतम आकार। |
|
|  | allowIncorrectBarcodes | boolean | यह मान दर्शाता है कि गलत बारकोड्स की अनुमति है या नहीं। |
|
|  | codeTypes | java.lang.String[] | पढ़ने के लिए बारकोड के प्रकार। |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


वह मान प्राप्त करता है जो दर्शाता है कि क्या गलत बारकोड की अनुमति है।


**Returns:**
boolean -  true  यदि गलत बारकोड्स की अनुमति है; अन्यथा,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


बारकोड न्यूनतम तत्व का न्यूनतम आकार प्राप्त करता है।


**Returns:**
java.lang.Float - वह फ्लोट मान जो बारकोड के न्यूनतम तत्व को दर्शाता है;  null  यदि ऑटो मोड उपयोग किया गया है।

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


स्रोत छवि की गुणवत्ता प्राप्त करता है।


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


स्रोत बारकोड की गुणवत्ता प्राप्त करता है।


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


पृष्ठ क्षेत्रों को सम्मिलित करने वाले आयताकार क्षेत्र को प्राप्त करता है।


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


पढ़ने के लिए बारकोड प्रकार प्राप्त करता है।


**Returns:**
java.util.List<java.lang.String> - वह रीड‑ओनली संग्रह जो पढ़ने के लिए बारकोड के प्रकारों को रखता है; यदि सेट नहीं है तो खाली संग्रह।

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


वह मान सेट करता है जो दर्शाता है कि क्या गलत बारकोड की अनुमति है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  यदि गलत बारकोड्स की अनुमति है। |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


बारकोड न्यूनतम तत्व का न्यूनतम आकार सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dimension | java.lang.Float | बारकोड का न्यूनतम तत्व;  null  ऑटो मोड के लिए। |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


स्रोत छवि की गुणवत्ता सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | छवि गुणवत्ता मोड। |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


स्रोत बारकोड की गुणवत्ता सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | बारकोड गुणवत्ता मोड। |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


बारकोड वाले आयताकार क्षेत्र को सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | आयताकार क्षेत्र;  null  पूरे पृष्ठ को स्कैन करने के लिए। |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


पढ़ने के लिए बारकोड प्रकार सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | बारकोड के प्रकार;  null  या सभी प्रकारों के लिए खाली। |
|

