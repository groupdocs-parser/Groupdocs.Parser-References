---
title: "OcrEventHandler"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر معالجًا لأحداث OCR."
type: docs
weight: 26
url: /ar/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

يوفر معالجًا لأحداث OCR.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | ينشئ مثيلاً جديدًا من الفئة [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | يحصل على قائمة برسائل التحذير. |
|
|  | [hasWarnings()](#hasWarnings--) | يحصل على القيمة التي تشير إلى ما إذا كانت قائمة التحذيرات غير فارغة. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | يعيد قائمة برسائل التحذير للصفحة ذات الفهرس pageIndex. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | يضبط رسائل التحذير للصفحة. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


ينشئ مثيلاً جديدًا من الفئة [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


يحصل على قائمة برسائل التحذير.


**Returns:**
java.util.List<java.lang.String> - قائمة برسائل التحذير لجميع الصفحات.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


يحصل على القيمة التي تشير إلى ما إذا كانت قائمة التحذيرات غير فارغة.


**Returns:**
boolean -  true  إذا لم تكن قائمة التحذيرات فارغة؛ وإلا،  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


يعيد قائمة برسائل التحذير للصفحة ذات الفهرس pageIndex.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|

**Returns:**
java.util.List<java.lang.String> - قائمة برسائل التحذير للصفحة؛ قائمة فارغة إذا لم توجد رسائل تحذير للصفحة.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


يضبط رسائل التحذير للصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة الذي يبدأ من الصفر. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | قائمة رسائل التحذير للصفحة. |
|

