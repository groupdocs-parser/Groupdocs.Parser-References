---
title: "Size"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل حجمًا."
type: docs
weight: 28
url: /ar/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

يمثل حجمًا.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | ينشئ مثيلاً جديداً من فئة [Size](../../com.groupdocs.parser.data/size). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getWidth()](#getWidth--) | يحصل على العرض. |
|
|  | [getHeight()](#getHeight--) | يحصل على الارتفاع. |
|
|  | [isEmpty()](#isEmpty--) | يحصل على قيمة تشير إلى ما إذا كان الحجم فارغاً. |
|
|  | [parse(String s)](#parse-java.lang.String-) | يحوّل تمثيل السلسلة لحجم إلى ما يعادله من الفئة. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


ينشئ مثيلاً جديداً من فئة [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العرض | double | العرض بالبكسل. |
|
|  | الارتفاع | double | الارتفاع بالبكسل. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


يحصل على العرض.


**Returns:**
double - قيمة مزدوجة تمثل العرض بالبكسل.

### getHeight() {#getHeight--}
```
public double getHeight()
```


يحصل على الارتفاع.


**Returns:**
double - قيمة مزدوجة تمثل الارتفاع بالبكسل.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


يحصل على قيمة تشير إلى ما إذا كان الحجم فارغاً.


**Returns:**
boolean -  true  إذا كان  العرض  والارتفاع  صفرًا؛ وإلا،  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


يقوم بتحويل تمثيل السلسلة لحجم إلى ما يعادله من فئة. قيمة الإرجاع تشير إلى ما إذا كان التحويل ناجحًا أم فاشلًا.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | s | java.lang.String | سلسلة تحتوي على حجم للتحويل. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
