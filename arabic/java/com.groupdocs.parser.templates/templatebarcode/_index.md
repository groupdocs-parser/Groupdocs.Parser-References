---
title: "TemplateBarcode"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر حقل الباركود القالب."
type: docs
weight: 11
url: /ar/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

يوفر حقل الباركود القالب.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) مع اسم بأحرف كبيرة. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) مع اسم بأحرف كبيرة. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب. |
|
|  | الاسم | java.lang.String | اسم حقل الباركود. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) مع اسم بأحرف كبيرة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب. |
|
|  | الاسم | java.lang.String | اسم حقل الباركود. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) مع اسم بأحرف كبيرة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب. |
|
|  | الاسم | java.lang.String | اسم حقل الباركود. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب. |
|
|  | الاسم | java.lang.String | اسم حقل الباركود. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


يقوم بتهيئة نسخة جديدة من الفئة [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب. |
|
|  | الاسم | java.lang.String | اسم حقل الباركود. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة التي تحتوي على حقل الباركود في القالب.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


ينشئ نسخة من العنصر الحالي مع تعديل جميع الإحداثيات وفقًا للمعامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| العامل | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
