---
title: "TemplateTable"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر جدول القالب."
type: docs
weight: 20
url: /ar/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

يوفر جدول القالب.

هناك طريقتان لتعريف جدول:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | يُنشئ مثيلًا جديدًا من فئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) بالاسم UPPER CASE. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | يُنشئ مثيلًا جديدًا من فئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) بالاسم UPPER CASE. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | يُنشئ مثيلًا جديدًا من فئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) بالاسم UPPER CASE. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getLayout()](#getLayout--) | يحصل على تخطيط الجدول. |
|
|  | [getParameters()](#getParameters--) | يحصل على المعلمات لاكتشاف الجدول في الوضع التلقائي. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


يُنشئ مثيلًا جديدًا من فئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) بالاسم UPPER CASE.

يتم تعيين جدول القالب بواسطة تخطيط الجدول إذا تعذر اكتشاف الجدول تلقائيًا:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | تخطيط الجدول. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


يُنشئ مثيلًا جديدًا من فئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) بالاسم UPPER CASE.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | تخطيط الجدول. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | تخطيط الجدول. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | تخطيط الجدول. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


يُنشئ مثيلًا جديدًا من فئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) بالاسم UPPER CASE.

إذا تم تعيين جدول القالب بواسطة معلمات الكاشف، يتم اكتشاف الجدول تلقائيًا:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


يُنشئ مثيلاً جديدًا للفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | المعلمات لاكتشاف الجدول في الوضع التلقائي. |
|
|  | الاسم | java.lang.String | اسم الجدول. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يقع فيها جدول القالب؛  null  إذا كان جدول القالب موجودًا في أي صفحة. |
|
|  | pageWidth | java.lang.Double | عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|
|  | useUpperCaseName | boolean | القيمة التي تشير إلى ما إذا كان  name  يتم تحويله إلى الأحرف الكبيرة. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


يحصل على تخطيط الجدول.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


يحصل على المعلمات لاكتشاف الجدول في الوضع التلقائي.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
