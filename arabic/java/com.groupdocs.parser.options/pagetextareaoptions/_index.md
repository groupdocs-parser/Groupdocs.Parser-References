---
title: "PageTextAreaOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لاستخراج مناطق نص الصفحة."
type: docs
weight: 32
url: /ar/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

يوفر الخيارات المستخدمة لاستخراج مناطق نص الصفحة.

يتم استخدام نسخة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) كمعامل في [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
وطرق [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-). راجع أمثلة الاستخدام هناك.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) بالقيم الافتراضية. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع خيار استخدام OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع القدرة على تعيين خيارات OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) باستخدام التعبير النمطي. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) باستخدام التعبير النمطي والمساحة المستطيلة. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) باستخدام التعبير النمطي، والمساحة المستطيلة، وحجم الحدود المتجاهلة. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) بحجم الحدود المتجاهلة. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getExpression()](#getExpression--) | يحصل على التعبير النمطي. |
|
|  | [isMatchCase()](#isMatchCase--) | يحصل على القيمة التي تشير إلى ما إذا كانت حالة النص غير متجاهلة. |
|
|  | [isUniteSegments()](#isUniteSegments--) | يحصل على القيمة التي تشير إلى ما إذا كانت القطاعات موحدة. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | يحصل على القيمة التي تشير إلى ما إذا كان تنسيق النص متجاهلاً. |
|
|  | [isUseOcr()](#isUseOcr--) | يحصل على القيمة التي تشير إلى ما إذا كان موصل OCR يُستخدم لاستخراج نص. |
|
|  | [getOcrOptions()](#getOcrOptions--) | يحصل على الخيارات الإضافية لوظيفة OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) بالقيم الافتراضية.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع خيار استخدام OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | useOcr | boolean | القيمة التي تشير إلى ما إذا كانت وظيفة OCR تُستخدم لاستخراج نص. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع القدرة على تعيين خيارات OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | useOcr | boolean | القيمة التي تشير إلى ما إذا كانت وظيفة OCR تُستخدم لاستخراج نص. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | الخيارات الإضافية لوظيفة OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) باستخدام التعبير النمطي. يتم تعيين الخيارات الأخرى افتراضيًا (انظر الملاحظات للتفاصيل).

الخصائص التالية لها قيم افتراضية:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) باستخدام التعبير النمطي والمساحة المستطيلة. يتم تعيين الخيارات الأخرى افتراضيًا (انظر الملاحظات للتفاصيل).

الخصائص التالية لها قيم افتراضية:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) باستخدام التعبير النمطي، والمساحة المستطيلة، وحجم الحدود المتجاهلة. يتم تعيين الخيارات الأخرى افتراضيًا (انظر الملاحظات للتفاصيل).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|
|  | rectangleTolerance | double | حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة جزء من ارتفاع عنصر النص. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | uniteSegments | boolean | القيمة التي تشير إلى ما إذا كانت المقاطع موحدة. |
|
|  | ignoreFormatting | boolean | القيمة التي تشير إلى ما إذا كان تنسيق النص متجاهلاً. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


ينشئ نسخة جديدة من الفئة [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) بحجم الحدود المتجاهلة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | uniteSegments | boolean | القيمة التي تشير إلى ما إذا كانت المقاطع موحدة. |
|
|  | ignoreFormatting | boolean | القيمة التي تشير إلى ما إذا كان تنسيق النص متجاهلاً. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|
|  | rectangleTolerance | double | حجم الحد الذي يتم تجاهله عند التقاطه بواسطة المنطقة المستطيلة. يتم قياسه بنسبة جزء من ارتفاع عنصر النص. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


يحصل على التعبير النمطي.


**Returns:**
java.lang.String - سلسلة تمثل التعبير النمطي.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


يحصل على القيمة التي تشير إلى ما إذا كانت حالة النص غير متجاهلة.


**Returns:**
boolean -  true  إذا لم يتم تجاهل حالة النص؛ وإلا،  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


يحصل على القيمة التي تشير إلى ما إذا كانت القطاعات موحدة.


**Returns:**
boolean - {code true} إذا كانت المقاطع موحدة؛ وإلا، {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


يحصل على القيمة التي تشير إلى ما إذا كان تنسيق النص متجاهلاً.


**Returns:**
boolean -  true  إذا كان تنسيق النص متجاهلاً؛ وإلا،  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


يحصل على القيمة التي تشير إلى ما إذا كان موصل OCR يُستخدم لاستخراج نص.


**Returns:**
منطقي -  true  إذا كانت وظيفة OCR مُستخدمة؛ وإلا،  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


يحصل على الخيارات الإضافية لوظيفة OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

