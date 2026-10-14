---
title: "PageTableAreaCell"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل خلية جدول تُستخدم في الفئة."
type: docs
weight: 23
url: /ar/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

يمثل خلية جدول تُستخدم في الفئة [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | يُنشئ مثيلًا جديدًا للفئة [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | يُنشئ مثيلًا جديدًا للفئة [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | يحصل على فهرس الصف. |
|
|  | [getColumnIndex()](#getColumnIndex--) | يحصل على فهرس العمود. |
|
|  | [getRowSpan()](#getRowSpan--) | يحصل على العدد الإجمالي للصفوف التي تحتوي على خلية الجدول. |
|
|  | [getColumnSpan()](#getColumnSpan--) | يحصل على العدد الإجمالي للأعمدة التي تحتوي على خلية الجدول. |
|
|  | [getPageArea()](#getPageArea--) | يحصل على قيمة خلية الجدول. |
|
|  | [getText()](#getText--) | يحصل على قيمة نص خلية الجدول. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


يُنشئ مثيلًا جديدًا للفئة [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rowIndex | int | الفهرس الصفري للصف. |
|
|  | columnIndex | int | الفهرس الصفري للعمود. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | قيمة خلية الجدول. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


يُنشئ مثيلًا جديدًا للفئة [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rowIndex | int | الفهرس الصفري للصف. |
|
|  | columnIndex | int | الفهرس الصفري للعمود. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | قيمة خلية الجدول. |
|
|  | rowSpan | int | العدد الإجمالي للصفوف التي تحتوي على خلية الجدول. |
|
|  | columnSpan | int | العدد الإجمالي للأعمدة التي تحتوي على خلية الجدول. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


يحصل على فهرس الصف.


**Returns:**
int - فهرس صفري للصف الأول الذي يحتوي على خلية الجدول.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


يحصل على فهرس العمود.


**Returns:**
int - فهرس صفري للعمود الأول الذي يحتوي على خلية الجدول.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


يحصل على العدد الإجمالي للصفوف التي تحتوي على خلية الجدول.


**Returns:**
int - قيمة عدد صحيح موجبة تمثل العدد الإجمالي للصفوف التي تحتوي على خلية الجدول.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


يحصل على العدد الإجمالي للأعمدة التي تحتوي على خلية الجدول.


**Returns:**
int - قيمة عدد صحيح موجبة تمثل العدد الإجمالي للأعمدة التي تحتوي على خلية الجدول.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


يحصل على قيمة خلية الجدول.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


يحصل على قيمة نص خلية الجدول.


**Returns:**
java.lang.String - سلسلة تمثل قيمة نصية للخلية؛  null  إذا لم تحتوي الخلية على قيمة نصية.

