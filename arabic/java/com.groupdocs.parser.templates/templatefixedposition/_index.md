---
title: "TemplateFixedPosition"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر موضع حقل القالب المحدد بالمنطقة المستطيلة."
type: docs
weight: 13
url: /ar/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

يوفر موضع حقل القالب المحدد بالمنطقة المستطيلة.

هذه هي أبسط طريقة لتحديد موضع الحقل. يتطلب تعيين منطقة مستطيلة على الصفحة التي تحدد
قيمة الحقل. سيتم استخراج كل النص الموجود (حتى جزئياً) داخل المنطقة المستطيلة كقيمة:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | ينشئ مثيلاً جديداً من الفئة [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) class. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة التي تحتوي على حقل القالب. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


ينشئ مثيلاً جديداً من الفئة [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) class.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على حقل القالب. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة التي تحتوي على حقل القالب.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


ينشئ نسخة من الموضع الحالي مع تعديل جميع الإحداثيات وفق العامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| العامل | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
