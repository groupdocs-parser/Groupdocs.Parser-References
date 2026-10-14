---
title: "PageBarcodeArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل منطقة باركود الصفحة التي تُستخدم لتمثيل قيمة الباركود في وظيفة التحليل باستخدام القالب."
type: docs
weight: 18
url: /ar/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object، [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

يمثل منطقة باركود الصفحة التي تُستخدم لتمثيل قيمة الباركود في وظيفة التحليل باستخدام القالب.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | يفّتح مثيلًا جديدًا من الفئة [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getValue()](#getValue--) | يحصل على قيمة الباركود. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | يحصل على اسم نوع الباركود. |
|
|  | [getConfidence()](#getConfidence--) | يحصل على مستوى الثقة للباركود المُحلل. |
|
|  | [getAngle()](#getAngle--) | يحصل على زاوية الباركود. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


يفّتح مثيلًا جديدًا من الفئة [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | قيمة الباركود. |
|
|  | codeTypeName | java.lang.String | اسم نوع الباركود. |
|
|  | confidence | int | مستوى الثقة للباركود المُحلل. |
|
|  | angle | double | زاوية الباركود. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على منطقة الباركود. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على منطقة الباركود. |
|

### getValue() {#getValue--}
```
public String getValue()
```


يحصل على قيمة الباركود.


**Returns:**
java.lang.String - قيمة نصية تمثل قيمة منطقة صفحة الباركود.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


يحصل على اسم نوع الباركود.


**Returns:**
java.lang.String - قيمة نصية تمثل اسم نوع الباركود.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


يحصل على مستوى الثقة للباركود المُحلل.


**Returns:**
int - قيمة عددية تمثل ثقة الباركود المُحلل (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


يحصل على زاوية الباركود.


**Returns:**
double - قيمة عددية تمثل زاوية الباركود (0-360).

