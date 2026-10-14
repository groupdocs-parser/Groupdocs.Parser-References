---
title: "OcrConnectorBase"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر وظائف OCR."
type: docs
weight: 25
url: /ar/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

يوفر وظائف OCR.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | ينشئ مثلاً جديداً من الفئة [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج النص مدعومًا. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | يحصل على القيمة التي تشير إلى ما إذا كان استخراج مناطق النص مدعومًا. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | التعرف على نص من  imageStream  تدفق. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | التعرف على مناطق النص من  imageStream  تدفق. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


ينشئ مثلاً جديداً من الفئة [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج النص مدعومًا.


**Returns:**
boolean -  true  إذا كان استخراج النص مدعومًا؛ وإلا،  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


يحصل على القيمة التي تشير إلى ما إذا كان استخراج مناطق النص مدعومًا.


**Returns:**
boolean -  true  إذا كانت مناطق استخراج النص مدعومة؛ وإلا،  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


التعرف على نص من  imageStream  تدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | تمثيل الصورة لصفحة المستند. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | خيارات OCR. |
|

**Returns:**
java.lang.String - سلسلة تمثل نصًا تم التعرف عليه؛  null  إذا لم يكن التعرف على النص مدعومًا.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


التعرف على مناطق النص من  imageStream  تدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | تمثيل الصورة لصفحة المستند. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | حجم صفحة المستند. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | خيارات OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - مجموعة من كائنات [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)؛  null  إذا لم يكن التعرف على مناطق النص مدعومًا.

