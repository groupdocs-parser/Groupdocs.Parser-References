---
title: "TemplateOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة في التحليل بواسطة وظيفة القالب."
type: docs
weight: 17
url: /ar/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

يوفر الخيارات المستخدمة في التحليل بواسطة وظيفة القالب.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | ينشئ مثلاً جديداً من الفئة [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | يحصل على حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


ينشئ مثلاً جديداً من الفئة [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangleTolerance | double | حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة جزء من ارتفاع عنصر النص. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


يحصل على حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة جزء من ارتفاع عنصر النص.


**Returns:**
double - القيمة العشرية من 0 (بدون حد) إلى 1 (تجاهل العنصر بالكامل).

