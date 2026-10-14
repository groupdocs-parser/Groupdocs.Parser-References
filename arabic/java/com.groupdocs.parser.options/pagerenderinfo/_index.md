---
title: "PageRenderInfo"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات كيفية عرض الصفحة."
type: docs
weight: 30
url: /ar/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

يمثل معلومات كيفية عرض الصفحة.

بعض المستندات (مثل جداول البيانات، على سبيل المثال) لا يمكنها عرض صفحة
كصورة واحدة. بالنسبة لتلك المستندات يتم عرض الصفحة كمجموعة من البلاطات.
يتم وضع هذه البلاطات في الجدول المستطيل.


RowCount
و
ColumnCount
تمثل إجمالي عدد الصفوف والأعمدة
من هذا الجدول. إذا تم عرض صفحة المستند كصورة واحدة تكون هذه الخصائص مساوية لـ 1.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | يُنشئ مثيلاً جديدًا من الفئة [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | يحصل على رقم الصفحة. |
|
|  | [getRowCount()](#getRowCount--) | احصل على إجمالي عدد صفوف البلاطات. |
|
|  | [getColumnCount()](#getColumnCount--) | احصل على إجمالي عدد أعمدة البلاطات. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | يعيد فهرس العمود حيث تم وضع البلاطة ذات  tileIndex  . |
|
|  | [getRow(int tileIndex)](#getRow-int-) | يعيد فهرس الصف حيث تم وضع البلاطة ذات  tileIndex  . |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


يُنشئ مثيلاً جديدًا من الفئة [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageNumber | int | عدد الصفحة (يبدأ من 1). |
|
|  | rowCount | int | إجمالي عدد صفوف البلاط. |
|
|  | columnCount | int | إجمالي عدد أعمدة البلاط. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


يحصل على رقم الصفحة.


**Returns:**
int - القيمة الصحيحة التي تمثل رقم الصفحة (يبدأ من 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


احصل على إجمالي عدد صفوف البلاطات.


**Returns:**
int - القيمة الصحيحة التي تمثل إجمالي عدد صفوف البلاط.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


احصل على إجمالي عدد أعمدة البلاطات.


**Returns:**
int - القيمة الصحيحة التي تمثل إجمالي عدد أعمدة البلاط.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


يعيد فهرس العمود حيث تم وضع البلاطة ذات  tileIndex  .


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | tileIndex | int | الفهرس الصفري للبلاطة. |
|

**Returns:**
int - القيمة الصحيحة الصفرية التي تمثل فهرس العمود.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


يعيد فهرس الصف حيث تم وضع البلاطة ذات  tileIndex  .


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | tileIndex | int | الفهرس الصفري للبلاطة. |
|

**Returns:**
int - القيمة الصحيحة الصفرية التي تمثل فهرس الصف.

