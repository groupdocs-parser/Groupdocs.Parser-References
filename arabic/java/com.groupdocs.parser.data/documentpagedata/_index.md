---
title: "DocumentPageData"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل بيانات صفحة المستند."
type: docs
weight: 12
url: /ar/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

يمثل بيانات صفحة المستند. يتكون من كائنات [FieldData](../../com.groupdocs.parser.data/fielddata) التي تحتوي على بيانات الحقول من صفحة المستند.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | يفّتح مثيلًا جديدًا من الفئة [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | يحصل على فهرس الصفحة. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


يفّتح مثيلًا جديدًا من الفئة [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الحقول | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | مجموعة بيانات الحقول. |
|
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


يحصل على فهرس الصفحة.


**Returns:**
int - فهرس الصفحة يبدأ من الصفر.

