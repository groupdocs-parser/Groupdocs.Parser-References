---
title: "OcrOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لموصل OCR."
type: docs
weight: 27
url: /ar/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

يوفر الخيارات المستخدمة لموصل OCR.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع القيم الافتراضية. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع مساحة مستطيلة. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع خيارات معاينة الصفحة. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع كائن [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع مساحة مستطيلة وكائن [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المساحة المستطيلة التي تقيد مساحة الصفحة المستخدمة في التعرف على النص. |
|
|  | [getHandler()](#getHandler--) | يحصل على معالج الحدث لالتقاط أحداث OCR. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | يحصل على القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | يحصل على خيارات معاينة الصفحة المستخدمة لتصيير الصفحة التي تُغذى إلى محرك OCR. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | يضبط خيارات معاينة الصفحة المستخدمة لتصيير الصفحة التي تُغذى إلى محرك OCR. |
|
|  | [getLanguage()](#getLanguage--) | يحصل على اللغة المستخدمة للتعرف الضوئي على الأحرف. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | يضبط اللغة المستخدمة للتعرف الضوئي على الأحرف. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | يضبط المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | يضبط معالج الحدث لالتقاط أحداث OCR. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | يضبط القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع القيم الافتراضية.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع مساحة مستطيلة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع خيارات معاينة الصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | الخيارات المستخدمة لتصيير معاينة الصفحة التي تُغذى إلى محرك OCR. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع كائن [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | مثال من [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) لالتقاط أحداث OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions) مع مساحة مستطيلة وكائن [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | مثال من [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) لالتقاط أحداث OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


ينشئ مثيلاً جديدًا من الفئة [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | مثال من [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) لالتقاط أحداث OCR. |
|
|  | useSpellCheker | boolean | القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المساحة المستطيلة التي تقيد مساحة الصفحة المستخدمة في التعرف على النص.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


يحصل على معالج الحدث لالتقاط أحداث OCR.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


يحصل على القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا.


**Returns:**
منطقي -  true  إذا كان مدقق الإملاء مستخدمًا؛ وإلا،  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


يحصل على خيارات معاينة الصفحة المستخدمة لتصيير الصفحة التي تُغذى إلى محرك OCR.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


يضبط خيارات معاينة الصفحة المستخدمة لتصيير الصفحة التي تُغذى إلى محرك OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | خيارات معاينة الصفحة. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


يحصل على اللغة المستخدمة للتعرف الضوئي على الأحرف.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


يضبط اللغة المستخدمة للتعرف الضوئي على الأحرف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | قيمة تعداد [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


يضبط المنطقة المستطيلة التي تقيد مساحة الصفحة المستخدمة للتعرف على النص.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المستطيل، أو  null  لمسح الصفحة بالكامل. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


يضبط معالج الحدث لالتقاط أحداث OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | معالج الحدث. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


يضبط القيمة التي تشير إلى ما إذا كان مدقق الإملاء مستخدمًا.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  لتمكين تدقيق الإملاء. |
|

