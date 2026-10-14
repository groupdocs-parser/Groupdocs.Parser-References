---
title: "Size"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "एक आकार का प्रतिनिधित्व करता है।"
type: docs
weight: 28
url: /hi/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

एक आकार का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | [Size](../../com.groupdocs.parser.data/size) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getWidth()](#getWidth--) | चौड़ाई प्राप्त करता है। |
|
|  | [getHeight()](#getHeight--) | ऊँचाई प्राप्त करता है। |
|
|  | [isEmpty()](#isEmpty--) | एक मान प्राप्त करता है जो दर्शाता है कि आकार खाली है या नहीं। |
|
|  | [parse(String s)](#parse-java.lang.String-) | एक आकार की स्ट्रिंग प्रतिनिधित्व को उसके क्लास समकक्ष में परिवर्तित करता है। |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


[Size](../../com.groupdocs.parser.data/size) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | चौड़ाई | double | पिक्सेल में चौड़ाई। |
|
|  | ऊँचाई | double | पिक्सेल में ऊँचाई। |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


चौड़ाई प्राप्त करता है।


**Returns:**
double - एक डबल मान जो पिक्सेल में चौड़ाई का प्रतिनिधित्व करता है।

### getHeight() {#getHeight--}
```
public double getHeight()
```


ऊँचाई प्राप्त करता है।


**Returns:**
double - एक डबल मान जो पिक्सेल में ऊँचाई का प्रतिनिधित्व करता है।

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


एक मान प्राप्त करता है जो दर्शाता है कि आकार खाली है या नहीं।


**Returns:**
boolean -  true  यदि चौड़ाई और ऊँचाई शून्य हैं; अन्यथा,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


आकार की स्ट्रिंग प्रतिनिधित्व को उसके क्लास समकक्ष में परिवर्तित करता है। एक रिटर्न वैल्यू यह दर्शाता है कि परिवर्तन सफल हुआ या विफल।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | s | java.lang.String | परिवर्तित करने के लिए आकार वाली एक स्ट्रिंग। |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
