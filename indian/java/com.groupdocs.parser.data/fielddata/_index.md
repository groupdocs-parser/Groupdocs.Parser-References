---
title: "FieldData"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "फ़ील्ड डेटा का प्रतिनिधित्व करता है जैसे नाम, पेज इंडेक्स, फ़ील्ड वैल्यू आदि।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

फ़ील्ड डेटा का प्रतिनिधित्व करता है जैसे नाम, पेज इंडेक्स, फ़ील्ड वैल्यू आदि। फ़ील्ड के आधार पर वैल्यू टेक्स्ट, इमेज, टेबल आदि हो सकती है।

[FieldData](../../com.groupdocs.parser.data/fielddata) क्लास के इंस्टेंस को [DocumentData](../../com.groupdocs.parser.data/documentdata) कलेक्शन में उपयोग किया जाता है।

## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getName()](#getName--) | फ़ील्ड का नाम प्राप्त करता है। |
|
|  | [getPageIndex()](#getPageIndex--) | पेज इंडेक्स प्राप्त करता है। |
|
|  | [getPageArea()](#getPageArea--) | फ़ील्ड का मान प्राप्त करता है। |
|
|  | [getLinkedField()](#getLinkedField--) | लिंक्ड फ़ील्ड प्राप्त करता है। |
|
|  | [getText()](#getText--) | टेक्स्ट प्राप्त करता है। |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या  Name  को बड़े अक्षरों में बदला गया था। |
|
### getName() {#getName--}
```
public String getName()
```


फ़ील्ड का नाम प्राप्त करता है।


**Returns:**
java.lang.String - एक अपरकेस स्ट्रिंग वैल्यू जो फ़ील्ड के नाम का प्रतिनिधित्व करती है।

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


पेज इंडेक्स प्राप्त करता है।


**Returns:**
int - वह ज़ीरो-आधारित इंडेक्स जो उस पेज को दर्शाता है जिसमें फ़ील्ड मौजूद है।

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


फ़ील्ड का मान प्राप्त करता है।

फ़ील्ड के आधार पर PageArea प्रॉपर्टी में [PageArea](../../com.groupdocs.parser.data/pagearea) क्लास के किसी भी इनहेरिटर को शामिल किया जा सकता है।
उदाहरण के लिए, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) मेथड केवल टेक्स्ट फ़ील्ड्स को एक्सट्रैक्ट करता है।

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


लिंक्ड फ़ील्ड प्राप्त करता है।


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


टेक्स्ट प्राप्त करता है।


**Returns:**
java.lang.String - एक स्ट्रिंग वैल्यू जो फ़ील्ड टेक्स्ट के मान का प्रतिनिधित्व करती है; यदि [PageArea](../../com.groupdocs.parser.data/pagearea) प्रॉपर्टी [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) नहीं है तो null।

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या  Name  को बड़े अक्षरों में बदला गया था।


**Returns:**
boolean - एक बूलियन मान जो दर्शाता है कि क्या  Name  को बड़े अक्षरों में बदला गया था।

