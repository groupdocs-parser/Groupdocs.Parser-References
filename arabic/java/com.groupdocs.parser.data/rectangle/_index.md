---
title: "مستطيل"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل مساحة مستطيلة."
type: docs
weight: 26
url: /ar/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

يمثل مساحة مستطيلة.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | ينشئ مثيلاً جديداً من الفئة [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | ينشئ مثيلاً جديداً من الفئة [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getLeft()](#getLeft--) | يحصل على إحداثي x للحافة اليسرى للمنطقة المستطيلة. |
|
|  | [getTop()](#getTop--) | يحصل على إحداثي y للحافة العلوية للمنطقة المستطيلة. |
|
|  | [getRight()](#getRight--) | يحصل على إحداثي x للحافة اليمنى للمنطقة المستطيلة. |
|
|  | [getBottom()](#getBottom--) | يحصل على إحداثي y للحافة السفلية للمنطقة المستطيلة. |
|
|  | [getPosition()](#getPosition--) | يحصل على إحداثيات الزاوية العلوية اليسرى للمنطقة المستطيلة. |
|
|  | [getSize()](#getSize--) | يحصل على الحجم. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


ينشئ مثيلاً جديداً من الفئة [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | اليسار | double | إحداثي x للحافة اليسرى للمنطقة المستطيلة. |
|
|  | الأعلى | double | إحداثي y للحافة العلوية للمنطقة المستطيلة. |
|
|  | يمين | double | إحداثي x للحافة اليمنى للمنطقة المستطيلة. |
|
|  | أسفل | double | إحداثي y للحافة السفلية للمنطقة المستطيلة. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


ينشئ مثيلاً جديداً من الفئة [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | إحداثيات الزاوية العلوية اليسرى للمنطقة المستطيلة. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | حجم المنطقة المستطيلة. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


يحصل على إحداثي x للحافة اليسرى للمنطقة المستطيلة.


**Returns:**
double - قيمة مزدوجة تمثل إحداثي x للحافة اليسرى للمنطقة المستطيلة.

### getTop() {#getTop--}
```
public double getTop()
```


يحصل على إحداثي y للحافة العلوية للمنطقة المستطيلة.


**Returns:**
double - قيمة مزدوجة تمثل إحداثي y للحافة العلوية للمنطقة المستطيلة.

### getRight() {#getRight--}
```
public double getRight()
```


يحصل على إحداثي x للحافة اليمنى للمنطقة المستطيلة.


**Returns:**
double - قيمة مزدوجة تمثل إحداثي x للحافة اليمنى للمنطقة المستطيلة.

### getBottom() {#getBottom--}
```
public double getBottom()
```


يحصل على إحداثي y للحافة السفلية للمنطقة المستطيلة.


**Returns:**
double - قيمة مزدوجة تمثل إحداثي y للحافة السفلية للمنطقة المستطيلة.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


يحصل على إحداثيات الزاوية العلوية اليسرى للمنطقة المستطيلة.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


يحصل على الحجم.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
