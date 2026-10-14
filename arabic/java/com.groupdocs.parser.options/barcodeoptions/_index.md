---
title: "BarcodeOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات التي تُستخدم لاستخراج الباركود."
type: docs
weight: 10
url: /ar/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

يوفر الخيارات التي تُستخدم لاستخراج الباركود.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | ينشئ مثيلًا جديدًا من فئة BarcodeOptions بالقيم الافتراضية. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | ينشئ مثيلًا جديدًا من فئة BarcodeOptions بالمنطقة المستطيلة. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | ينشئ مثيلًا جديدًا من فئة BarcodeOptions بإعدادات الجودة وأنواع الرموز. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | ينشئ مثيلًا جديدًا من فئة BarcodeOptions. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | يحصل على القيمة التي تشير إلى ما إذا كانت الباركودات غير الصحيحة مسموحة. |
|
|  | [getDimension()](#getDimension--) | يحصل على الحد الأدنى لحجم العنصر الأدنى للباركود. |
|
|  | [getImageQuality()](#getImageQuality--) | يحصل على جودة الصورة المصدر. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | يحصل على جودة الباركود المصدر. |
|
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة التي تحتوي على مناطق الصفحة. |
|
|  | [getCodeTypes()](#getCodeTypes--) | يحصل على أنواع الباركود للقراءة. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | يضبط القيمة التي تشير إلى ما إذا كانت الباركودات غير الصحيحة مسموحة. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | يضبط الحد الأدنى لحجم العنصر الأدنى للباركود. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | يضبط جودة الصورة المصدر. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | يضبط جودة الباركود المصدر. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | يضبط المنطقة المستطيلة التي تحتوي على الباركود. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | يضبط أنواع الباركود للقراءة. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


ينشئ مثيلًا جديدًا من فئة BarcodeOptions بالقيم الافتراضية.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


ينشئ مثيلًا جديدًا من فئة BarcodeOptions بالمنطقة المستطيلة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الباركود. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


ينشئ مثيلًا جديدًا من فئة BarcodeOptions بإعدادات الجودة وأنواع الرموز.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | جودة الصورة المصدر. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | جودة الباركود المصدر. |
|
|  | codeTypes | java.lang.String[] | أنواع الباركود للقراءة. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


ينشئ مثيلًا جديدًا من فئة BarcodeOptions.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الباركود. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | جودة الصورة المصدر. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | جودة الباركود المصدر. |
|
|  | dimension | java.lang.Float | الحجم الأدنى للعنصر الأدنى للباركود. |
|
|  | allowIncorrectBarcodes | boolean | القيمة التي تشير إلى ما إذا كان السماح بالباركود غير الصحيح مسموحًا. |
|
|  | codeTypes | java.lang.String[] | أنواع الباركود للقراءة. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


يحصل على القيمة التي تشير إلى ما إذا كانت الباركودات غير الصحيحة مسموحة.


**Returns:**
منطقية -  true  إذا كان السماح بالباركود غير الصحيح مسموحًا؛ وإلا،  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


يحصل على الحد الأدنى لحجم العنصر الأدنى للباركود.


**Returns:**
java.lang.Float - القيمة العائمة التي تمثل العنصر الأدنى للباركود؛  null  إذا تم استخدام الوضع التلقائي.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


يحصل على جودة الصورة المصدر.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


يحصل على جودة الباركود المصدر.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة التي تحتوي على مناطق الصفحة.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


يحصل على أنواع الباركود للقراءة.


**Returns:**
java.util.List<java.lang.String> - المجموعة للقراءة فقط التي تحتوي على أنواع الباركود للقراءة؛ مجموعة فارغة إذا لم يتم تعيينها.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


يضبط القيمة التي تشير إلى ما إذا كانت الباركودات غير الصحيحة مسموحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  إذا كان السماح بالباركود غير الصحيح مسموحًا. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


يضبط الحد الأدنى لحجم العنصر الأدنى للباركود.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | dimension | java.lang.Float | العنصر الأدنى للباركود؛  null  للوضع التلقائي. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


يضبط جودة الصورة المصدر.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | وضع جودة الصورة. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


يضبط جودة الباركود المصدر.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | وضع جودة الباركود. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


يضبط المنطقة المستطيلة التي تحتوي على الباركود.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة؛  null  لمسح الصفحة بأكملها. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


يضبط أنواع الباركود للقراءة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | أنواع الباركود؛  null  أو فارغ لجميع الأنواع. |
|

