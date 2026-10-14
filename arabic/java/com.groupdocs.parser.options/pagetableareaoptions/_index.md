---
title: "PageTableAreaOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لاستخراج مناطق جداول الصفحة."
type: docs
weight: 31
url: /ar/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

يوفر الخيارات المستخدمة لاستخراج مناطق جداول الصفحة.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | ينشئ مثيلاً جديداً للفئة [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | ينشئ مثيلاً جديداً للفئة [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) مع مستطيل بحث ولا تخطيط ثابت. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | يحصل على تخطيط الجدول الذي يحدد الجدول في الصفحة. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


ينشئ مثيلاً جديداً للفئة [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | تخطيط الجدول الذي يحدد الجدول في الصفحة. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


ينشئ مثيلاً جديداً للفئة [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) مع مستطيل بحث ولا تخطيط ثابت.

مفيد لتقييد الجداول المكتشفة تلقائياً إلى منطقة من الصفحة. يعكس الـ C#

new PageTableAreaOptions(null) { Rectangle = ... }
نمط.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة على الصفحة حيث يجب اكتشاف الجداول؛ مرّر  null  للبحث في الصفحة بأكملها. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


يحصل على تخطيط الجدول الذي يحدد الجدول في الصفحة.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

