---
title: "SearchResult"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل نتيجة البحث في وظيفة البحث."
type: docs
weight: 27
url: /ar/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

يمثل نتيجة البحث في وظيفة البحث.

مثال من فئة SearchResult يُستخدم كقيمة إرجاع للطريقة [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-).
و[Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) الطرق. راجع أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | يُنشئ مثيلًا جديدًا من الفئة [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | يُنشئ مثيلًا جديدًا من الفئة [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getPosition()](#getPosition--) | يحصل على الموضع في نص المستند. |
|
|  | [getText()](#getText--) | يحصل على النص. |
|
|  | [getPageIndex()](#getPageIndex--) | يحصل على فهرس الصفحة حيث تم العثور على النص. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | يحصل على التمييز الأيسر. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | يحصل على التمييز الأيمن. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | int | الموضع في نص المستند. |
|
|  | text | java.lang.String | النص الموجود. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة حيث تم العثور على النص. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | التمييز الأيسر. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | التمييز الأيمن. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | int | الموضع في نص المستند. |
|
|  | text | java.lang.String | النص الموجود. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة حيث تم العثور على النص. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


يحصل على الموضع في نص المستند.


**Returns:**
int - فهرس يبدأ من الصفر لموضع البداية لنتيجة البحث.

### getText() {#getText--}
```
public String getText()
```


يحصل على النص.


**Returns:**
java.lang.String - قيمة نصية تمثل النص الموجود.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


يحصل على فهرس الصفحة حيث تم العثور على النص.


**Returns:**
java.lang.Integer - فهرس يبدأ من الصفر للصفحة التي تم العثور فيها على النص؛  null  إذا تم البحث على كامل نص المستند.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


يحصل على التمييز الأيسر.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


يحصل على التمييز الأيمن.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

