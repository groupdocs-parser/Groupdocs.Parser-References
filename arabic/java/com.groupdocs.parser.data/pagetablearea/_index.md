---
title: "PageTableArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل منطقة جدول الصفحة التي تُستخدم لتمثيل جدول في وظيفة التحليل باستخدام القالب."
type: docs
weight: 22
url: /ar/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object، [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

يمثل منطقة جدول الصفحة التي تُستخدم لتمثيل جدول في وظيفة التحليل باستخدام القالب.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | ينشئ مثيلاً جديداً من الفئة [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getCells()](#getCells--) | يحصل على مجموعة الخلايا. |
|
|  | [getRowCount()](#getRowCount--) | يحصل على العدد الإجمالي لصفوف الجدول. |
|
|  | [getColumnCount()](#getColumnCount--) | يحصل على العدد الإجمالي لأعمدة الجدول. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | يعيد ارتفاع الصف. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | يعيد عرض العمود. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | يحصل على خلية الجدول حسب فهارس الصف والعمود. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


ينشئ مثيلاً جديداً من الفئة [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

ملاحظة: يحدد مشروع C# هذا المنشئ كـ
داخلي
(commit 954951f). في Java، "internal-to-the-assembly"
لا يترجم بشكل نظيف إلى package-private لأن المنتجين (
WordProcessingParser
,
TableAreaParser
,
إلخ.) توجد في
com.groupdocs.parser
, ليس
com.groupdocs.parser.data
. لذلك يُحافظ على هذا المنشئ

عام
حتى يظل إنشاء عبر الحزم يعمل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | صفوف | java.lang.Iterable<java.lang.Double> | مجموعة ارتفاعات الصفوف. |
|
|  | أعمدة | java.lang.Iterable<java.lang.Double> | مجموعة عرض الأعمدة. |
|
|  | خلايا | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | مجموعة الخلايا. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على الجدول. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الجدول. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


يحصل على مجموعة الخلايا. مجموعة قراءة فقط بسيطة من خلايا الجدول.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - مجموعة من خلايا الجدول

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


يحصل على العدد الإجمالي لصفوف الجدول.


**Returns:**
int - قيمة عددية صحيحة تحتوي على العدد الإجمالي لصفوف الجدول.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


يحصل على العدد الإجمالي لأعمدة الجدول.


**Returns:**
int - قيمة عددية صحيحة تحتوي على العدد الإجمالي لأعمدة الجدول.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


يعيد ارتفاع الصف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rowIndex | int | الفهرس الصفري للصف. |
|

**Returns:**
double - قيمة مزدوجة تمثل ارتفاع الصف.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


يعيد عرض العمود.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | columnIndex | int | الفهرس الصفري للعمود. |
|

**Returns:**
double - قيمة مزدوجة تمثل عرض العمود.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


يحصل على خلية الجدول حسب فهارس الصف والعمود.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rowIndex | int | الفهرس الصفري لصف الخلية. |
|
|  | columnIndex | int | الفهرس الصفري لعمود الخلية. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

