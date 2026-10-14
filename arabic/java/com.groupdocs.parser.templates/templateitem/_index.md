---
title: "TemplateItem"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر فئة أساسية مجردة لعناصر القالب."
type: docs
weight: 14
url: /ar/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

يوفر فئة أساسية مجردة لعناصر القالب.

المُشتقون من فئة [TemplateItem](../../com.groupdocs.parser.templates/templateitem) يُستخدمون في مجموعة [Template](../../com.groupdocs.parser.templates/template).

## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | ينشئ نسخة من العنصر الحالي مع تعديل جميع الإحداثيات وفقًا للمعامل المحدد. |
|
|  | [getName()](#getName--) | يحصل على اسم عنصر القالب. |
|
|  | [getPageIndex()](#getPageIndex--) | يحصل على فهرس الصفحة لعنصر القالب. |
|
|  | [getPageWidth()](#getPageWidth--) | يحصل على عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | يحصل على قيمة تشير إلى ما إذا كان  Name  قد تم تحويله إلى UPPER CASE. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


ينشئ نسخة من العنصر الحالي مع تعديل جميع الإحداثيات وفقًا للمعامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العامل | double | عامل القياس. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


يحصل على اسم عنصر القالب.


**Returns:**
java.lang.String - قيمة سلسلة بحروف كبيرة تمثل اسم عنصر القالب.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


يحصل على فهرس الصفحة لعنصر القالب.


**Returns:**
java.lang.Integer - قيمة عددية تمثل فهرس الصفحة التي يقع فيها عنصر القالب؛  null  إذا كان عنصر القالب موجودًا على أي صفحة.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


يحصل على عرض الصفحة التي تم استخدامها لإنشاء عنصر القالب.


**Returns:**
java.lang.Double - عرض الصفحة بالبكسل؛  null  إذا كان عرض الصفحة غير معروف.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


يحصل على قيمة تشير إلى ما إذا كان  Name  قد تم تحويله إلى UPPER CASE.


**Returns:**
boolean - قيمة منطقية تشير إلى ما إذا كان  Name  قد تم تحويله إلى UPPER CASE.

