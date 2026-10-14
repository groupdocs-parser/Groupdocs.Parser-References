---
title: "Page"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات صفحة المستند مثل فهرس الصفحة وحجم الصفحة."
type: docs
weight: 16
url: /ar/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

يمثل معلومات صفحة المستند مثل فهرس الصفحة وحجم الصفحة. يُستخدم لتمثيل الصفحة التي تحتوي على ورثة فئة [PageArea](../../com.groupdocs.parser.data/pagearea) في وظيفة التحليل باستخدام القالب.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | ينشئ مثيلاً جديداً من الفئة [Page](../../com.groupdocs.parser.data/page). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getIndex()](#getIndex--) | يحصل على فهرس الصفحة. |
|
|  | [getSize()](#getSize--) | يحصل على حجم الصفحة. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


ينشئ مثيلاً جديداً من الفئة [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | فهرس الصفحة. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | حجم الصفحة. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس الصفحة.


**Returns:**
int - فهرس الصفحة يبدأ من الصفر.

### getSize() {#getSize--}
```
public Size getSize()
```


يحصل على حجم الصفحة.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

