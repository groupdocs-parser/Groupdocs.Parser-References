---
title: "DocumentInfo"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات المستند."
type: docs
weight: 11
url: /ar/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

يمثل معلومات المستند.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## البناؤات

| البناء | الوصف |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getFileType()](#getFileType--) | يحصل على نوع المستند. |
|
|  | [getPageCount()](#getPageCount--) | يحصل على إجمالي عدد صفحات المستند. |
|
|  | [getRawPageCount()](#getRawPageCount--) | يحصل على إجمالي عدد الصفحات الخام للمستند. |
|
|  | [getSize()](#getSize--) | يحصل على حجم المستند بالبايت. |
|
|  | [getPages()](#getPages--) | يحصل على المعلومات حول الصفحات مثل الفهرس وحجم الصفحة. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


يحصل على نوع المستند.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


يحصل على إجمالي عدد صفحات المستند.


**Returns:**
int - قيمة عددية تمثل إجمالي عدد الصفحات.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


يحصل على إجمالي عدد الصفحات الخام للمستند.

استخدم خاصية [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) بدلاً من خاصية [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) لاستخراج النص الخام.
بعض المستندات لديها أرقام صفحات مختلفة في وضعية استخراج النص الدقيق والنص الخام.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - قيمة عددية تمثل إجمالي عدد الصفحات الخام.

### getSize() {#getSize--}
```
public abstract long getSize()
```


يحصل على حجم المستند بالبايت.


**Returns:**
long - قيمة عدد صحيح تمثل حجم المستند بالبايت.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


يحصل على المعلومات حول الصفحات مثل الفهرس وحجم الصفحة.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - مجموعة تحتوي على مثيلات من فئات [PageInfo](../../com.groupdocs.parser.options/pageinfo).

