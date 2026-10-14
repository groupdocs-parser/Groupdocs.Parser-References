---
title: "TemplateTableParameters"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر معلمات لخوارزميات اكتشاف الجدول."
type: docs
weight: 22
url: /ar/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

يوفر معلمات لخوارزميات اكتشاف الجدول.

هناك خوارزميتان لاكتشاف جدول:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

في بعض الحالات عندما لا تستطيع الخوارزميات اكتشاف جدول أو تقوم بذلك بطريقة غير دقيقة يتم استخدام الفئة [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | يُنشئ مثلاً جديداً من الفئة [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | يُنشئ مثلاً جديداً من الفئة [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة التي تحتوي على الجدول. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | يحصل على فواصل أعمدة الجدول. |
|
|  | [hasMergedCells()](#hasMergedCells--) | يحصل على القيمة التي تشير إلى ما إذا كان الجدول يحتوي على خلايا مدمجة. |
|
|  | [getMinRowCount()](#getMinRowCount--) | يحصل على الحد الأدنى لعدد صفوف الجدول. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | يحصل على الحد الأدنى لعدد أعمدة الجدول. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | يحصل على الحد الأدنى للمسافة بين أعمدة الجدول. |
|
|  | [scale(double factor)](#scale-double-) | ينشئ نسخة من هذه المعلمات مع تكبير جميع الإحداثيات بالعامل المحدد. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


يُنشئ مثلاً جديداً من الفئة [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الجدول. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | فواصل أعمدة الجدول. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


يُنشئ مثلاً جديداً من الفئة [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الجدول. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | فواصل أعمدة الجدول. |
|
|  | mergedCells | java.lang.Boolean | القيمة التي تشير إلى ما إذا كان الجدول يحتوي على خلايا مدمجة. |
|
|  | minRowCount | java.lang.Integer | الحد الأدنى لعدد صفوف الجدول. |
|
|  | minColumnCount | java.lang.Integer | الحد الأدنى لعدد أعمدة الجدول. |
|
|  | minVerticalSpace | java.lang.Integer | الحد الأدنى للمسافة بين أعمدة الجدول. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة التي تحتوي على الجدول.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


يحصل على فواصل أعمدة الجدول.


**Returns:**
java.util.List<java.lang.Double> - مجموعة من القيم المزدوجة التي تمثل إحداثيات x لفواصل أعمدة الجدول؛  null  إذا لم يتم تعيينها.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


يحصل على القيمة التي تشير إلى ما إذا كان الجدول يحتوي على خلايا مدمجة.


**Returns:**
java.lang.Boolean -  true  إذا كان الجدول يحتوي على خلايا مدمجة؛ وإلا،  false .  null  إذا لم يتم تعيينه.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


يحصل على الحد الأدنى لعدد صفوف الجدول.


**Returns:**
java.lang.Integer - قيمة عددية تمثل الحد الأدنى لعدد صفوف الجدول؛  null  إذا لم يتم تعيينها.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


يحصل على الحد الأدنى لعدد أعمدة الجدول.


**Returns:**
java.lang.Integer - قيمة عددية تمثل الحد الأدنى لعدد أعمدة الجدول؛  null  إذا لم يتم تعيينها.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


يحصل على الحد الأدنى للمسافة بين أعمدة الجدول.


**Returns:**
java.lang.Integer - قيمة عددية تمثل الحد الأدنى للمسافة بين أعمدة الجدول؛  null  إذا لم يتم تعيينها.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


ينشئ نسخة من هذه المعلمات مع تكبير جميع الإحداثيات بالعامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العامل | double | عامل القياس. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

