---
title: "PageGroupArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل مجموعة من مناطق الصفحة التي تُستخدم لتجميع أنواع مختلفة من كتل صفحة المستند في وظيفة التحليل باستخدام القالب."
type: docs
weight: 19
url: /ar/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object، [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

يمثل مجموعة من مناطق الصفحة التي تُستخدم لتجميع أنواع مختلفة من كتل صفحة المستند في وظيفة التحليل باستخدام القالب.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | ينشئ مثيلاً جديداً من الفئة [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getAreas()](#getAreas--) | يحصل على مجموعة المناطق الصفحية المجمعة. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


ينشئ مثيلاً جديداً من الفئة [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | مجموعة المناطق الصفحية التي سيتم تجميعها. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على المنطقة. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


يحصل على مجموعة المناطق الصفحية المجمعة.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - مجموعة من كائنات [PageArea](../../com.groupdocs.parser.data/pagearea).

