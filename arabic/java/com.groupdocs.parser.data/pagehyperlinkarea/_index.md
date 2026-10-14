---
title: "PageHyperlinkArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل منطقة صفحة تُستخدم لتمثيل ارتباط تشعبي على الصفحة."
type: docs
weight: 20
url: /ar/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object، [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

يمثل منطقة صفحة تُستخدم لتمثيل ارتباط تشعبي على الصفحة.

يتم استخدام نسخة من الفئة [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) كقيمة إرجاع للطرق التالية:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

انظر أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | يُنشئ نسخة جديدة من الفئة [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getText()](#getText--) | يحصل على نص الارتباط التشعبي. |
|
|  | [getUrl()](#getUrl--) | يحصل على عنوان URL للارتباط التشعبي. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


يُنشئ نسخة جديدة من الفئة [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | text | java.lang.String | نص الارتباط التشعبي. |
|
|  | url | java.lang.String | عنوان URL للارتباط التشعبي. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على الارتباط التشعبي. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الارتباط التشعبي. |
|

### getText() {#getText--}
```
public String getText()
```


يحصل على نص الارتباط التشعبي.


**Returns:**
java.lang.String - قيمة نصية تمثل نص الارتباط التشعبي.

### getUrl() {#getUrl--}
```
public String getUrl()
```


يحصل على عنوان URL للارتباط التشعبي.


**Returns:**
java.lang.String - قيمة نصية تمثل عنوان URL للارتباط التشعبي.

