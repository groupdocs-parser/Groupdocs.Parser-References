---
title: "Rectangle"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Dikdörtgen bir alanı temsil eder."
type: docs
weight: 26
url: /tr/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Dikdörtgen bir alanı temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Yeni bir [Rectangle](../../com.groupdocs.parser.data/rectangle) sınıf örneği başlatır. |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Yeni bir [Rectangle](../../com.groupdocs.parser.data/rectangle) sınıf örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getLeft()](#getLeft--) | Dikdörtgen alanın sol kenarının x koordinatını alır. |
|
|  | [getTop()](#getTop--) | Dikdörtgen alanın üst kenarının y koordinatını alır. |
|
|  | [getRight()](#getRight--) | Dikdörtgen alanın sağ kenarının x koordinatını alır. |
|
|  | [getBottom()](#getBottom--) | Dikdörtgen alanın alt kenarının y koordinatını alır. |
|
|  | [getPosition()](#getPosition--) | Dikdörtgen alanın sol üst köşesinin koordinatlarını alır. |
|
|  | [getSize()](#getSize--) | Boyutu alır. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Yeni bir [Rectangle](../../com.groupdocs.parser.data/rectangle) sınıf örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | sol | double | Dikdörtgen alanın sol kenarının x koordinatı. |
|
|  | üst | double | Dikdörtgen alanın üst kenarının y koordinatı. |
|
|  | sağ | double | Dikdörtgen alanın sağ kenarının x koordinatı. |
|
|  | alt | double | Dikdörtgen alanın alt kenarının y koordinatı. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Yeni bir [Rectangle](../../com.groupdocs.parser.data/rectangle) sınıf örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Dikdörtgen alanın sol üst köşesinin koordinatları. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Dikdörtgen alanın boyutu. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Dikdörtgen alanın sol kenarının x koordinatını alır.


**Returns:**
double - Dikdörtgen alanın sol kenarının x koordinatını temsil eden double değer.

### getTop() {#getTop--}
```
public double getTop()
```


Dikdörtgen alanın üst kenarının y koordinatını alır.


**Returns:**
double - Dikdörtgen alanın üst kenarının y koordinatını temsil eden double değer.

### getRight() {#getRight--}
```
public double getRight()
```


Dikdörtgen alanın sağ kenarının x koordinatını alır.


**Returns:**
double - Dikdörtgen alanın sağ kenarının x koordinatını temsil eden double değer.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Dikdörtgen alanın alt kenarının y koordinatını alır.


**Returns:**
double - Dikdörtgen alanın alt kenarının y koordinatını temsil eden double değer.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Dikdörtgen alanın sol üst köşesinin koordinatlarını alır.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Boyutu alır.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
