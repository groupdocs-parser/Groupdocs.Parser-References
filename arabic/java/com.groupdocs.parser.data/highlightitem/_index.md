---
title: "HighlightItem"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل تمييزًا لجزء من النص يُستخدم عادةً لشرح سياق النص الموجود في وظيفة البحث."
type: docs
weight: 14
url: /ar/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

يمثل تمييزًا، وهو جزء من النص يُستخدم عادةً لشرح سياق النص الموجود في وظيفة البحث.

مثال من فئة [HighlightItem](../../com.groupdocs.parser.data/highlightitem) يُستخدم كقيمة إرجاع للطريقة [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) ،
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | يُنشئ مثيلًا جديدًا من الفئة [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getPosition()](#getPosition--) | يحصل على الموضع في نص المستند. |
|
|  | [getText()](#getText--) | يحصل على نص التمييز. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


يُنشئ مثيلًا جديدًا من الفئة [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | position | int | الموضع في نص المستند. |
|
|  | text | java.lang.String | نص التمييز. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


يحصل على الموضع في نص المستند.


**Returns:**
int - فهرس يبدأ من الصفر لموضع البداية للتمييز.

### getText() {#getText--}
```
public String getText()
```


يحصل على نص التمييز.


**Returns:**
java.lang.String - قيمة نصية تمثل نص التمييز.

