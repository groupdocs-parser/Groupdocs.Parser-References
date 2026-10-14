---
title: "Point"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "एक बिंदु का प्रतिनिधित्व करता है।"
type: docs
weight: 25
url: /hi/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

एक बिंदु का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | [Point](../../com.groupdocs.parser.data/point) क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getX()](#getX--) | x-निर्देशांक प्राप्त करता है। |
|
|  | [getY()](#getY--) | y-निर्देशांक प्राप्त करता है। |
|
|  | [parse(String s)](#parse-java.lang.String-) | एक बिंदु के स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


[Point](../../com.groupdocs.parser.data/point) क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | x | double | x-निर्देशांक। |
|
|  | y | double | y-निर्देशांक। |
|

### getX() {#getX--}
```
public double getX()
```


x-निर्देशांक प्राप्त करता है।


**Returns:**
double - x-निर्देशांक को दर्शाने वाला दशमलव मान।

### getY() {#getY--}
```
public double getY()
```


y-निर्देशांक प्राप्त करता है।


**Returns:**
double - y-निर्देशांक को दर्शाने वाला दशमलव मान।

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


एक बिंदु की स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। एक रिटर्न वैल्यू यह दर्शाती है कि परिवर्तन सफल हुआ या विफल।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | s | java.lang.String | एक स्ट्रिंग जिसमें परिवर्तित करने के लिए बिंदु शामिल है। |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
