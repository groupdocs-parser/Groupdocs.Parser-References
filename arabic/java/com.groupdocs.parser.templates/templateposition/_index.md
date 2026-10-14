---
title: "TemplatePosition"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر فئة أساسية مجردة لمواقع القالب."
type: docs
weight: 18
url: /ar/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

يوفر فئة أساسية مجردة لمواقع القالب.

## البناؤات

| البناء | الوصف |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | ينشئ نسخة من الموضع الحالي مع تعديل جميع الإحداثيات وفق العامل المحدد. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


ينشئ نسخة من الموضع الحالي مع تعديل جميع الإحداثيات وفق العامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العامل | double | عامل القياس. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

