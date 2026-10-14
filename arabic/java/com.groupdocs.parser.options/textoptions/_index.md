---
title: "TextOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لاستخراج النص."
type: docs
weight: 37
url: /ar/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

يوفر الخيارات المستخدمة لاستخراج النص.

مثيل لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) يُستخدم كمعامل في [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
و[Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) الطرق. انظر أمثلة الاستخدام هناك.

يُستخدم لتحديد وضع النص الخام لاستخراج النص. النص في هذا الوضع يُستخرج بطريقة غير دقيقة
ولكن أسرع من الوضع القياسي. إذا لم يدعم وضع النص الخام تنسيق المستند،
فإن هذا المعامل يتم تجاهله ويُستخدم الوضع القياسي.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع خيار استخدام OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع القدرة على تعيين خيارات OCR. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | يحصل على القيمة التي تشير إلى ما إذا كان وضع النص الخام مُستخدمًا. |
|
|  | [isUseOcr()](#isUseOcr--) | يحصل على القيمة التي تشير إلى ما إذا كان موصل OCR يُستخدم لاستخراج نص. |
|
|  | [getOcrOptions()](#getOcrOptions--) | يحصل على الخيارات الإضافية لوظيفة OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | يحصل على القيمة التي تشير إلى ما إذا كانت التعليقات التوضيحية مُضمنة في النص المستخرج. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | يضبط القيمة التي تشير إلى ما إذا كانت التعليقات التوضيحية مُضمنة في النص المستخرج. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | القيمة التي تشير إلى ما إذا كان وضع النص الخام مُستخدمًا. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع خيار استخدام OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | القيمة التي تشير إلى ما إذا كان وضع النص الخام مُستخدمًا. |
|
|  | useOcr | boolean | القيمة التي تشير إلى ما إذا كانت وظيفة OCR تُستخدم لاستخراج نص. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


ينشئ مثيلًا جديدًا لفئة [TextOptions](../../com.groupdocs.parser.options/textoptions) مع القدرة على تعيين خيارات OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | القيمة التي تشير إلى ما إذا كان وضع النص الخام مُستخدمًا. |
|
|  | useOcr | boolean | القيمة التي تشير إلى ما إذا كانت وظيفة OCR تُستخدم لاستخراج نص. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | الخيارات الإضافية لوظيفة OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


يحصل على القيمة التي تشير إلى ما إذا كان وضع النص الخام مُستخدمًا.


**Returns:**
منطقي -  true  إذا كان وضع النص الخام مُستخدمًا؛ وإلا،  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


يحصل على القيمة التي تشير إلى ما إذا كانت التعليقات التوضيحية مُضمنة في النص المستخرج. القيمة الافتراضية هي  false .


**Returns:**
منطقي -  true  إذا كانت التعليقات التوضيحية مُضمنة؛ وإلا،  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


يضبط القيمة التي تشير إلى ما إذا كانت التعليقات التوضيحية مُضمنة في النص المستخرج.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  لتضمين التعليقات التوضيحية في النص المستخرج. |
|

