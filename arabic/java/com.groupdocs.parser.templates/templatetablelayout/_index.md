---
title: "TemplateTableLayout"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر تخطيط جدول القالب الذي يستخدمه الفئة لتحديد موضع الجدول."
type: docs
weight: 21
url: /ar/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

يوفر تخطيط جدول القالب الذي يستخدمه الفئة [TemplateTable](../../com.groupdocs.parser.templates/templatetable) لتحديد موضع الجدول.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | ينشئ مثيلاً جديداً للفئة [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة التي تحتوي على الجدول. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | يحصل على فواصل أعمدة الجدول. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | يحصل على فواصل صفوف الجدول. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | ينشئ تخطيطاً جديداً بنفس الحجم والفواصل والموضع في النقطة. |
|
|  | [scale(double factor)](#scale-double-) | ينشئ نسخة من هذا التخطيط مع تعديل جميع الإحداثيات وفق العامل المحدد. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


ينشئ مثيلاً جديداً للفئة [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | فواصل أعمدة الجدول. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | فواصل صفوف الجدول. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة التي تحتوي على الجدول.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


يحصل على فواصل أعمدة الجدول.


**Returns:**
java.util.List<java.lang.Double> - مجموعة من القيم المزدوجة التي تمثل إحداثيات x لفواصل أعمدة الجدول.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


يحصل على فواصل صفوف الجدول.


**Returns:**
java.util.List<java.lang.Double> - مجموعة من القيم المزدوجة التي تمثل إحداثيات y لفواصل صفوف الجدول.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


ينشئ تخطيطاً جديداً بنفس الحجم والفواصل والموضع في النقطة.

تتيح هذه الوظيفة نقل تخطيط الجدول.

على سبيل المثال، يحتوي المستند على جداول في كل صفحة (أو مجموعة من المستندات التي تحتوي على جدول في الصفحة).
تختلف هذه الجداول في الموقع والمحتوى، لكنها تحتوي على نفس الأعمدة والصفوف. في هذه الحالة المستخدم
يمكنه تعريف كائن [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) عند (0, 0) مرة واحدة ثم نقله إلى موقع الجدول المحدد.

إذا كان موقع الجدول يعتمد على كائن آخر في الصفحة، يمكن للمستخدم تعريف كائن [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)
استنادًا إلى مستند القالب ثم نقله وفقًا لكائن مرساة. على سبيل المثال، إذا كان هذا جدول ملخص
ويليه جدول تفاصيل (يمكن أن يحتوي على عدد مختلف من الصفوف). في هذه الحالة يمكن للمستخدم تعريف
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


`moveTo(Point)`
تُعيد الطريقة نسخة من الكائن الحالي. يمكن للمستخدم تمرير أي إحداثيات
(حتى السلبية - حينها سيتم نقل التخطيط إلى اليسار/الأعلى).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | موضع التخطيط الجديد. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


ينشئ نسخة من هذا التخطيط مع تعديل جميع الإحداثيات وفق العامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العامل | double | عامل القياس. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

