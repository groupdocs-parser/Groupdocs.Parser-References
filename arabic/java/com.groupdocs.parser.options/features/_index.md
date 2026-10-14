---
title: "الميزات"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل قائمة الميزات المدعومة."
type: docs
weight: 18
url: /ar/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

يمثل قائمة الميزات المدعومة. يسمح بالحصول على معلومات حول أي الميزات مدعومة أو غير مدعومة للمستند.

يتم استخدام نسخة من هذه الفئة كخاصية [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). راجع أمثلة الاستخدام هناك.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## البناؤات

| البناء | الوصف |
| --- | --- |
| [Features()](#Features--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | يعيد القيمة التي تشير إلى ما إذا كانت الميزة مدعومة. |
|
|  | [isText()](#isText--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج النص مدعومًا. |
|
|  | [isTextPage()](#isTextPage--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج صفحات النص مدعومًا. |
|
|  | [isFormattedText()](#isFormattedText--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج النص المنسق مدعومًا. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج صفحات النص المنسق مدعومًا. |
|
|  | [isSearch()](#isSearch--) | يحصل على القيمة التي تشير إلى ما إذا كان البحث في النص مدعومًا. |
|
|  | [isHighlight()](#isHighlight--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج التمييز مدعومًا. |
|
|  | [isBarcodes()](#isBarcodes--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج الباركودات مدعومًا. |
|
|  | [isToc()](#isToc--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج جدول المحتويات مدعومًا. |
|
|  | [isMetadata()](#isMetadata--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج البيانات الوصفية مدعومًا. |
|
|  | [isContainer()](#isContainer--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج الحاوية مدعومًا. |
|
|  | [isTextAreas()](#isTextAreas--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج مناطق النص مدعومًا. |
|
|  | [isStructure()](#isStructure--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج بنية النص مدعومًا. |
|
|  | [isImages()](#isImages--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج الصور مدعومًا. |
|
|  | [isHyperlinks()](#isHyperlinks--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج الروابط التشعبية مدعومًا. |
|
|  | [isTables()](#isTables--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج الجداول مدعومًا. |
|
|  | [isAnnotations()](#isAnnotations--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج التعليقات التوضيحية مدعومًا. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | يحصل على القيمة التي تشير إلى ما إذا كان التحليل باستخدام القالب مدعومًا. |
|
|  | [isParseForm()](#isParseForm--) | يحصل على القيمة التي تشير إلى ما إذا كان تحليل النماذج مدعومًا. |
|
|  | [isPreview()](#isPreview--) | يحصل على القيمة التي تشير إلى ما إذا كان إنشاء المعاينة مدعومًا. |
|
|  | [isPagePreview()](#isPagePreview--) | يحصل على القيمة التي تشير إلى ما إذا كان إنشاء معاينة الصفحة مدعومًا. |
|
|  | [isOcr()](#isOcr--) | يحصل على القيمة التي تشير إلى ما إذا كانت وظيفة OCR مدعومة. |
|
|  | [isWorksheet()](#isWorksheet--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج ورقة العمل مدعومًا. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


يعيد القيمة التي تشير إلى ما إذا كانت الميزة مدعومة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | featureName | java.lang.String | اسم الميزة. |
|

**Returns:**
boolean -  true  إذا كانت الميزة مدعومة؛ وإلا،  false .

### isText() {#isText--}
```
public boolean isText()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج النص مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج النص مدعومًا؛ وإلا،  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج صفحات النص مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج صفحة النص مدعومًا؛ وإلا،  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج النص المنسق مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج النص المنسق مدعومًا؛ وإلا،  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج صفحات النص المنسق مدعومًا.


**Returns:**
boolean -  true  إذا كانت صفحة النص المنسق مدعومة؛ وإلا،  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


يحصل على القيمة التي تشير إلى ما إذا كان البحث في النص مدعومًا.


**Returns:**
boolean -  true  إذا كان البحث النصي مدعومًا؛ وإلا،  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج التمييز مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج التمييز مدعومًا؛ وإلا،  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج الباركودات مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج الباركود مدعومًا؛ وإلا،  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج جدول المحتويات مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج جدول المحتويات مدعومًا؛ وإلا،  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج البيانات الوصفية مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج البيانات الوصفية مدعومًا؛ وإلا،  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج الحاوية مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج الحاوية مدعومًا؛ وإلا،  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج مناطق النص مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج مناطق النص مدعومًا؛ وإلا،  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج بنية النص مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج بنية النص مدعومًا؛ وإلا،  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج الصور مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج الصور مدعومًا؛ وإلا،  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج الروابط التشعبية مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج الروابط التشعبية مدعومًا؛ وإلا،  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج الجداول مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج الجداول مدعومًا؛ وإلا،  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج التعليقات التوضيحية مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج التعليقات التوضيحية مدعومًا؛ وإلا،  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


يحصل على القيمة التي تشير إلى ما إذا كان التحليل باستخدام القالب مدعومًا.


**Returns:**
boolean -  true  إذا كان التحليل حسب القالب مدعومًا؛ وإلا،  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


يحصل على القيمة التي تشير إلى ما إذا كان تحليل النماذج مدعومًا.


**Returns:**
منطقي - true إذا كان تحليل النماذج مدعومًا؛ وإلا false.

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


يحصل على القيمة التي تشير إلى ما إذا كان إنشاء المعاينة مدعومًا.


**Returns:**
منطقي - true إذا كان توليد المعاينة مدعومًا؛ وإلا false.

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


يحصل على القيمة التي تشير إلى ما إذا كان إنشاء معاينة الصفحة مدعومًا.


**Returns:**
منطقي - true إذا كان توليد معاينة الصفحة مدعومًا؛ وإلا false.

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


يحصل على القيمة التي تشير إلى ما إذا كانت وظيفة OCR مدعومة.


**Returns:**
منطقي - true إذا كانت وظيفة OCR مدعومة؛ وإلا false.

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج ورقة العمل مدعومًا.


**Returns:**
منطقي - true إذا كان استخراج ورقة العمل مدعومًا؛ وإلا false.

