---
title: "HighlightOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات التي تُستخدم لاستخراج كتلة نصية مميزة حول النص الموجود في سيناريوهات البحث."
type: docs
weight: 22
url: /ar/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

يوفر الخيارات المستخدمة لاستخراج تمييز (كتلة نصية حول النص الموجود في سيناريوهات البحث).

يتم استخدام مثيل من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) كمعامل في طريقة [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
انظر أمثلة الاستخدام هناك.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) دون تحديد أي حدود. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) تُستخدم لاستخراج تمييز بطول ثابت. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) تُستخدم لاستخراج تمييز محدود بالسطر. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) تُستخدم لاستخراج تمييز بعدد كلمات ثابت. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | يحصل على الحد الأقصى لطول النص. |
|
|  | [getWordCount()](#getWordCount--) | يحصل على الحد الأقصى لعدد الكلمات. |
|
|  | [isLineLimited()](#isLineLimited--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | يضبط الحد الأقصى لطول النص. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | يضبط الحد الأقصى لعدد الكلمات. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | يضبط القيمة التي تشير إلى ما إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) دون تحديد أي حدود. قم بتعيين واحد على الأقل من #setMaxLength(Integer).setMaxLength(Integer)، #setWordCount(Integer).setWordCount(Integer)، #setLineLimited(boolean).setLineLimited(boolean) قبل تمريره إلى المحلل.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) تُستخدم لاستخراج تمييز بطول ثابت.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | maxLength | int | الحد الأقصى لطول النص. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) تُستخدم لاستخراج تمييز محدود بالسطر.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | الحد الأقصى لطول النص. |
|
|  | isLineLimited | boolean | القيمة التي تشير إلى ما إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) تُستخدم لاستخراج تمييز بعدد كلمات ثابت.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | الحد الأقصى لطول النص. |
|
|  | wordCount | int | العدد الأقصى للكلمات. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


ينشئ مثيلًا جديدًا من فئة [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | الحد الأقصى لطول النص. |
|
|  | wordCount | java.lang.Integer | العدد الأقصى للكلمات. |
|
|  | isLineLimited | boolean | القيمة التي تشير إلى ما إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


يحصل على الحد الأقصى لطول النص.


**Returns:**
java.lang.Integer - قيمة عدد صحيح موجبة تمثل الحد الأقصى لطول النص؛  null  إذا لم يكن طول النص محدودًا.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


يحصل على الحد الأقصى لعدد الكلمات.


**Returns:**
java.lang.Integer - قيمة عدد صحيح موجبة تمثل الحد الأقصى لعدد الكلمات؛  null  إذا لم يكن عدد الكلمات محدودًا.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص.


**Returns:**
boolean -  true  إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص؛ وإلا،  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


يضبط الحد الأقصى لطول النص.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | عدد صحيح غير سالب؛  null  لإزالة حد الطول. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


يضبط الحد الأقصى لعدد الكلمات.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | عدد صحيح غير سالب؛  null  لإزالة حد عدد الكلمات. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


يضبط القيمة التي تشير إلى ما إذا كان استخراج التمييز محدودًا ببداية (أو نهاية) سطر النص.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | lineLimited | boolean | true  لتقييد الحدود حسب السطر. |
|

