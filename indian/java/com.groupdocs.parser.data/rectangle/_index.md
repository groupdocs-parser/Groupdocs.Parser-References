---
title: "Rectangle"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "एक आयताकार क्षेत्र का प्रतिनिधित्व करता है।"
type: docs
weight: 26
url: /hi/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

एक आयताकार क्षेत्र का प्रतिनिधित्व करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | नए [Rectangle](../../com.groupdocs.parser.data/rectangle) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | नए [Rectangle](../../com.groupdocs.parser.data/rectangle) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getLeft()](#getLeft--) | आयताकार क्षेत्र के बाएँ किनारे का x-निर्देशांक प्राप्त करता है। |
|
|  | [getTop()](#getTop--) | आयताकार क्षेत्र के शीर्ष किनारे का y-निर्देशांक प्राप्त करता है। |
|
|  | [getRight()](#getRight--) | आयताकार क्षेत्र के दाएँ किनारे का x-निर्देशांक प्राप्त करता है। |
|
|  | [getBottom()](#getBottom--) | आयताकार क्षेत्र के नीचे किनारे का y-निर्देशांक प्राप्त करता है। |
|
|  | [getPosition()](#getPosition--) | आयताकार क्षेत्र के ऊपरी-बाएँ कोने के निर्देशांक प्राप्त करता है। |
|
|  | [getSize()](#getSize--) | आकार प्राप्त करता है। |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


नए [Rectangle](../../com.groupdocs.parser.data/rectangle) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | बाएँ | double | आयताकार क्षेत्र के बाएँ किनारे का x-निर्देशांक। |
|
|  | ऊपर | double | आयताकार क्षेत्र के शीर्ष किनारे का y-निर्देशांक। |
|
|  | दाएँ | double | आयताकार क्षेत्र के दाएँ किनारे का x-निर्देशांक। |
|
|  | नीचे | double | आयताकार क्षेत्र के नीचे किनारे का y-निर्देशांक। |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


नए [Rectangle](../../com.groupdocs.parser.data/rectangle) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | आयताकार क्षेत्र के ऊपरी-बाएँ कोने के निर्देशांक। |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | आयताकार क्षेत्र का आकार। |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


आयताकार क्षेत्र के बाएँ किनारे का x-निर्देशांक प्राप्त करता है।


**Returns:**
double - एक डबल मान जो आयताकार क्षेत्र के बाएँ किनारे के x-निर्देशांक को दर्शाता है।

### getTop() {#getTop--}
```
public double getTop()
```


आयताकार क्षेत्र के शीर्ष किनारे का y-निर्देशांक प्राप्त करता है।


**Returns:**
double - एक डबल मान जो आयताकार क्षेत्र के शीर्ष किनारे के y-निर्देशांक को दर्शाता है।

### getRight() {#getRight--}
```
public double getRight()
```


आयताकार क्षेत्र के दाएँ किनारे का x-निर्देशांक प्राप्त करता है।


**Returns:**
double - एक डबल मान जो आयताकार क्षेत्र के दाएँ किनारे के x-निर्देशांक को दर्शाता है।

### getBottom() {#getBottom--}
```
public double getBottom()
```


आयताकार क्षेत्र के नीचे किनारे का y-निर्देशांक प्राप्त करता है।


**Returns:**
double - एक डबल मान जो आयताकार क्षेत्र के नीचे किनारे के y-निर्देशांक को दर्शाता है।

### getPosition() {#getPosition--}
```
public Point getPosition()
```


आयताकार क्षेत्र के ऊपरी-बाएँ कोने के निर्देशांक प्राप्त करता है।


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


आकार प्राप्त करता है।


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
