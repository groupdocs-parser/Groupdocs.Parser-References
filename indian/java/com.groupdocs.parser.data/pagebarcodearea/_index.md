---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में बारकोड मान को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ बारकोड क्षेत्र का प्रतिनिधित्व करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में बारकोड मान को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ बारकोड क्षेत्र का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | नए उदाहरण को प्रारंभ करता है [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getValue()](#getValue--) | बारकोड मान प्राप्त करता है। |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | बारकोड प्रकार का नाम प्राप्त करता है। |
|
|  | [getConfidence()](#getConfidence--) | पार्स किए गए बारकोड की विश्वसनीयता स्तर प्राप्त करता है। |
|
|  | [getAngle()](#getAngle--) | बारकोड का कोण प्राप्त करता है। |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


नए उदाहरण को प्रारंभ करता है [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | बारकोड का मान। |
|
|  | codeTypeName | java.lang.String | बारकोड का प्रकार नाम। |
|
|  | confidence | int | पार्स किए गए बारकोड की विश्वसनीयता स्तर। |
|
|  | angle | double | बारकोड का कोण। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | वह पृष्ठ जिसमें बारकोड क्षेत्र शामिल है। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | वह आयताकार क्षेत्र जिसमें बारकोड क्षेत्र शामिल है। |
|

### getValue() {#getValue--}
```
public String getValue()
```


बारकोड मान प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो बारकोड पृष्ठ क्षेत्र के मान का प्रतिनिधित्व करता है।

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


बारकोड प्रकार का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो बारकोड के प्रकार नाम का प्रतिनिधित्व करता है।

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


पार्स किए गए बारकोड की विश्वसनीयता स्तर प्राप्त करता है।


**Returns:**
int - पार्स किए गए बारकोड की विश्वसनीयता को दर्शाने वाला पूर्णांक मान (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


बारकोड का कोण प्राप्त करता है।


**Returns:**
double - बारकोड के कोण को दर्शाने वाला दशमलव मान (0-360).

