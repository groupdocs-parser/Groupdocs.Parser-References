---
title: "Point"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل نقطة."
type: docs
weight: 25
url: /ar/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

يمثل نقطة.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | يُنشئ نسخة جديدة من الفئة [Point](../../com.groupdocs.parser.data/point). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getX()](#getX--) | يحصل على إحداثي x. |
|
|  | [getY()](#getY--) | يحصل على إحداثي y. |
|
|  | [parse(String s)](#parse-java.lang.String-) | يحوّل تمثيل النص للنقطة إلى ما يعادلها من فئة. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


يُنشئ نسخة جديدة من الفئة [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | x | double | إحداثي x. |
|
|  | y | double | إحداثي y. |
|

### getX() {#getX--}
```
public double getX()
```


يحصل على إحداثي x.


**Returns:**
double - قيمة مزدوجة تمثل إحداثي x.

### getY() {#getY--}
```
public double getY()
```


يحصل على إحداثي y.


**Returns:**
double - قيمة مزدوجة تمثل إحداثي y.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


يقوم بتحويل تمثيل السلسلة لنقطة إلى ما يعادلها من الفئة. قيمة الإرجاع تشير إلى ما إذا كان التحويل ناجحًا أم فاشلًا.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | s | java.lang.String | سلسلة تحتوي على نقطة للتحويل. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
