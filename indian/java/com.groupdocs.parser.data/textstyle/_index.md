---
title: "TextStyle"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "पाठ की शैली का प्रतिनिधित्व करता है जैसे फ़ॉन्ट नाम, फ़ॉन्ट आकार आदि।"
type: docs
weight: 30
url: /hi/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

टेक्स्ट की शैली का प्रतिनिधित्व करता है जैसे फ़ॉन्ट नाम, फ़ॉन्ट आकार आदि।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | [TextStyle](../../com.groupdocs.parser.data/textstyle) क्लास का नया उदाहरण इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getName()](#getName--) | शैली का नाम प्राप्त करता है। |
|
|  | [getFontName()](#getFontName--) | फ़ॉन्ट का नाम प्राप्त करता है। |
|
|  | [getFontSize()](#getFontSize--) | फ़ॉन्ट आकार प्राप्त करता है। |
|
|  | [isBold()](#isBold--) | फ़ॉन्ट बोल्ड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [isItalic()](#isItalic--) | फ़ॉन्ट इटैलिक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


[TextStyle](../../com.groupdocs.parser.data/textstyle) क्लास का नया उदाहरण इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | नाम | java.lang.String | स्टाइल का नाम। |
|
|  | fontName | java.lang.String | फ़ॉन्ट का नाम। |
|
|  | fontSize | double | फ़ॉन्ट का आकार। |
|
|  | bold | boolean | फ़ॉन्ट बोल्ड है या नहीं, यह दर्शाने वाला मान। |
|
|  | italic | boolean | फ़ॉन्ट इटैलिक है या नहीं, यह दर्शाने वाला मान। |
|

### getName() {#getName--}
```
public String getName()
```


शैली का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो स्टाइल नाम का प्रतिनिधित्व करता है।

### getFontName() {#getFontName--}
```
public String getFontName()
```


फ़ॉन्ट का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग मान जो फ़ॉन्ट नाम का प्रतिनिधित्व करता है।

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


फ़ॉन्ट आकार प्राप्त करता है।


**Returns:**
double - एक डबल मान जो फ़ॉन्ट आकार का प्रतिनिधित्व करता है।

### isBold() {#isBold--}
```
public boolean isBold()
```


फ़ॉन्ट बोल्ड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि फ़ॉन्ट बोल्ड है; अन्यथा,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


फ़ॉन्ट इटैलिक है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean -  true  यदि फ़ॉन्ट इटैलिक है; अन्यथा,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
