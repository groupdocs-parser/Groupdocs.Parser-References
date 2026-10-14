---
title: "PageTextArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل منطقة نص الصفحة التي تُستخدم لتمثيل قيمة نصية في وظيفة التحليل باستخدام القالب أو وظيفة تحليل النماذج."
type: docs
weight: 24
url: /ar/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object، [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

يمثل منطقة نص الصفحة التي تُستخدم لتمثيل قيمة نصية في وظيفة التحليل باستخدام القالب أو وظيفة تحليل النماذج.

يتم استخدام نسخة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) كقيمة إرجاع للطرق التالية:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

كما يتم استخدام نسخة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) كقيمة لخاصية [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

انظر أمثلة الاستخدام هناك.

يمكن أن تكون مساحة النص مفردة أو مركبة. في الحالة الأولى تحتوي على نص محاط بمنطقة مستطيلة.
في الحالة الثانية تحتوي على مساحات نصية أخرى؛ يتم حساب خصائص النص والجدول بواسطة مساحات النص الفرعية.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | يقوم بتهيئة نسخة جديدة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | يقوم بتهيئة نسخة جديدة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | يقوم بتهيئة نسخة جديدة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getText()](#getText--) | يحصل على النص. |
|
|  | [getBaseLine()](#getBaseLine--) | يحصل على الخط الأساسي. |
|
|  | [getTextStyle()](#getTextStyle--) | يحصل على نمط النص مثل حجم الخط، اسم الخط، وما إلى ذلك. |
|
|  | [getAreas()](#getAreas--) | يحصل على مجموعة مناطق صفحات النص الفرعية. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


يقوم بتهيئة نسخة جديدة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | text | java.lang.String | قيمة النص. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على مساحة النص. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مساحة النص. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


يقوم بتهيئة نسخة جديدة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | text | java.lang.String | قيمة النص. |
|
|  | baseLine | java.lang.Double | الخط الأساسي للنص. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | نمط النص. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على مساحة النص. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مساحة النص. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


يقوم بتهيئة نسخة جديدة من فئة [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | مجموعة مساحات صفحات النص الفرعية. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على مساحة النص. |
|

### getText() {#getText--}
```
public String getText()
```


يحصل على النص.


**Returns:**
java.lang.String - قيمة سلسلة تمثل قيمة مساحة صفحة النص.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


يحصل على الخط الأساسي.


**Returns:**
double - قيمة مزدوجة تمثل الخط الأساسي.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


يحصل على نمط النص مثل حجم الخط، اسم الخط، وما إلى ذلك.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


يحصل على مجموعة مناطق صفحات النص الفرعية.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - مجموعة من مساحات صفحات النص الفرعية؛ تكون فارغة إذا لم يكن لمساحة صفحة النص أطفال.

