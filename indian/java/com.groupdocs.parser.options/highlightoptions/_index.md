---
title: "HighlightOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "खोज परिदृश्यों में पाए गए पाठ के आसपास एक ब्लॉक को हाइलाइट करने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

खोज परिदृश्यों में पाए गए टेक्स्ट के आसपास के टेक्स्ट ब्लॉक (हाइलाइट) को निकालने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

एक उदाहरण [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का उपयोग [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) मेथड में पैरामीटर के रूप में किया जाता है।
वहाँ उपयोग उदाहरण देखें।

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | कोई सीमा सेट किए बिना [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | स्थिर-लंबाई हाइलाइट निकालने के लिए उपयोग की जाने वाली [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | लाइन-सीमित हाइलाइट निकालने के लिए उपयोग की जाने वाली [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | स्थिर शब्द गणना के साथ हाइलाइट निकालने के लिए उपयोग की जाने वाली [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है। |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | अधिकतम पाठ लंबाई प्राप्त करता है। |
|
|  | [getWordCount()](#getWordCount--) | अधिकतम शब्द गणना प्राप्त करता है। |
|
|  | [isLineLimited()](#isLineLimited--) | एक मान प्राप्त करता है जो दर्शाता है कि हाइलाइट निष्कर्षण पाठ लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं। |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | अधिकतम पाठ लंबाई सेट करता है। |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | अधिकतम शब्द गणना सेट करता है। |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | एक मान सेट करता है जो दर्शाता है कि हाइलाइट निष्कर्षण पाठ लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं। |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


कोई सीमा सेट किए बिना [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है। पार्सर को पास करने से पहले #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) में से कम से कम एक सेट करें।


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


स्थिर-लंबाई हाइलाइट निकालने के लिए उपयोग की जाने वाली [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | maxLength | int | अधिकतम पाठ लंबाई। |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


लाइन-सीमित हाइलाइट निकालने के लिए उपयोग की जाने वाली [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | अधिकतम पाठ लंबाई। |
|
|  | isLineLimited | boolean | वह मान जो दर्शाता है कि हाइलाइट निष्कर्षण टेक्स्ट लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं। |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


स्थिर शब्द गणना के साथ हाइलाइट निकालने के लिए उपयोग की जाने वाली [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | अधिकतम पाठ लंबाई। |
|
|  | wordCount | int | अधिकतम शब्द गणना। |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) क्लास का नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | अधिकतम पाठ लंबाई। |
|
|  | wordCount | java.lang.Integer | अधिकतम शब्द गणना। |
|
|  | isLineLimited | boolean | वह मान जो दर्शाता है कि हाइलाइट निष्कर्षण टेक्स्ट लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं। |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


अधिकतम पाठ लंबाई प्राप्त करता है।


**Returns:**
java.lang.Integer - अधिकतम पाठ लंबाई को दर्शाने वाला एक सकारात्मक पूर्णांक मान;  null  यदि पाठ लंबाई सीमित नहीं है।

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


अधिकतम शब्द गणना प्राप्त करता है।


**Returns:**
java.lang.Integer - अधिकतम शब्द गणना को दर्शाने वाला एक सकारात्मक पूर्णांक मान;  null  यदि शब्द गणना सीमित नहीं है।

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


एक मान प्राप्त करता है जो दर्शाता है कि हाइलाइट निष्कर्षण पाठ लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं।


**Returns:**
boolean -  true  यदि हाइलाइट निष्कर्षण टेक्स्ट लाइन की शुरुआत (या अंत) द्वारा सीमित है; अन्यथा,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


अधिकतम पाठ लंबाई सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | एक गैर-नकारात्मक पूर्णांक;  null  लंबाई सीमा हटाने के लिए। |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


अधिकतम शब्द गणना सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | एक गैर-नकारात्मक पूर्णांक;  null  शब्द-गणना सीमा हटाने के लिए। |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


एक मान सेट करता है जो दर्शाता है कि हाइलाइट निष्कर्षण पाठ लाइन की शुरुआत (या अंत) द्वारा सीमित है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lineLimited | boolean | true  लाइन सीमाओं द्वारा सीमित करने के लिए। |
|

