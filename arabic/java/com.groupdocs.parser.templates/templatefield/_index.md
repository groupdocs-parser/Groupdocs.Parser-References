---
title: "TemplateField"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر حقل النص القالب."
type: docs
weight: 12
url: /ar/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

يوفر حقل النص القالب.

يتم تعريف حقول النص وفق موضعها على الصفحة. هناك ثلاث طرق لتعريف حقل نصي:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) class. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) بالاسم بأحرف كبيرة. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) بالاسم بأحرف كبيرة. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) class. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) class. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getPosition()](#getPosition--) | يحصل على القيمة التي تصف كيفية العثور على حقل القالب في صفحة المستند. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) class.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | موضع الحقل. |
|
|  | الاسم | java.lang.String | اسم الحقل. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) بالاسم بأحرف كبيرة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | موضع الحقل. |
|
|  | الاسم | java.lang.String | اسم الحقل. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) بالاسم بأحرف كبيرة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | موضع الحقل. |
|
|  | الاسم | java.lang.String | اسم الحقل. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) class.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | موضع الحقل. |
|
|  | الاسم | java.lang.String | اسم الحقل. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


ينشئ مثيلاً جديداً من الفئة [TemplateField](../../com.groupdocs.parser.templates/templatefield) class.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | موضع الحقل. |
|
|  | الاسم | java.lang.String | اسم الحقل. |
|
|  | pageIndex | java.lang.Integer | قيمة عددية صحيحة تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛ null إذا كان عنصر القالب يقع في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


يحصل على القيمة التي تصف كيفية العثور على حقل القالب في صفحة المستند.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

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
