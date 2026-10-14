---
title: "PageAreaOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لاستخراج مناطق الصفحة."
type: docs
weight: 28
url: /ar/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

يوفر الخيارات المستخدمة لاستخراج مناطق الصفحة.

يُستخدم كائن من فئة [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) كمعامل في [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
وطرق [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). راجع أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | يُنشئ مثيلًا جديدًا من فئة [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) مع حجم الحد المتجاهل. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | يُنشئ مثيلًا جديدًا من فئة [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | يحصل على حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


يُنشئ مثيلًا جديدًا من فئة [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) مع حجم الحد المتجاهل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


يُنشئ مثيلًا جديدًا من فئة [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|
|  | rectangleTolerance | double | حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة جزء من ارتفاع عنصر النص. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة التي تحتوي على مناطق الصفحة.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


يحصل على حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة جزء من ارتفاع عنصر النص.


**Returns:**
double - القيمة العشرية من 0 (بدون حد) إلى 1 (تجاهل العنصر بالكامل).

