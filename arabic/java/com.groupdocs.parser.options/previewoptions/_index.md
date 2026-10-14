---
title: "PreviewOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر خيارات لتعيين المتطلبات ومندوبين التدفق لإنشاء المعاينة."
type: docs
weight: 34
url: /ar/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

يوفر خيارات لتعيين المتطلبات ومندوبين التدفق لإنشاء المعاينة.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | يُنشئ نسخة جديدة من الفئة [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) مما يؤدي إلى إغلاق تدفق الإخراج. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | يُنشئ نسخة جديدة من الفئة [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) مما يؤدي إلى إرجاع تدفق الإخراج إلى العميل للاستخدام لاحقًا. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getWidth()](#getWidth--) | يحصل على عرض معاينة الصفحة. |
|
|  | [setWidth(int width)](#setWidth-int-) | يضبط عرض معاينة الصفحة. |
|
|  | [getHeight()](#getHeight--) | يحصل على ارتفاع معاينة الصفحة. |
|
|  | [setHeight(int height)](#setHeight-int-) | يضبط ارتفاع معاينة الصفحة. |
|
|  | [getDpi()](#getDpi--) | يحصل على dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | يضبط dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | يحصل على مصفوفة أرقام الصفحات لتوليد المعاينات. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | يضبط مصفوفة أرقام الصفحات لتوليد المعاينات. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | يحصل على تنسيق صورة المعاينة. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | يضبط تنسيق صورة المعاينة. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | يحصل على نسخة من المندوب لإنشاء تدفق الصفحة. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | يضبط نسخة من المندوب لإنشاء تدفق الصفحة. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | يحصل على نسخة من المندوب لإكمال معاينة الصفحة. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | يضبط نسخة من المندوب لإكمال معاينة الصفحة. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | يحصل على نسخة من المندوب لمعلومات عرض معاينة الصفحة. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | يضبط نسخة من المندوب لمعلومات عرض معاينة الصفحة. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


يُنشئ نسخة جديدة من الفئة [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) مما يؤدي إلى إغلاق تدفق الإخراج.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | ينشئ تدفقًا لمعاينة صفحة محددة. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


يُنشئ نسخة جديدة من الفئة [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) مما يؤدي إلى إرجاع تدفق الإخراج إلى العميل للاستخدام لاحقًا.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | ينشئ تدفقًا لمعاينة صفحة محددة |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | يُخطر بأن توليد معاينة الصفحة انتهى ويحصل على تدفق الإخراج. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


يحصل على عرض معاينة الصفحة.


**Returns:**
int - عرض الصفحة.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


يضبط عرض معاينة الصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العرض | int | عرض الصفحة. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


يحصل على ارتفاع معاينة الصفحة.


**Returns:**
int - ارتفاع الصفحة.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


يضبط ارتفاع معاينة الصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الارتفاع | int | ارتفاع الصفحة. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


يحصل على dpi.


**Returns:**
int - قيمة عددية تمثل dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


يضبط dpi.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | dpi | int | دقة النقاط. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


يحصل على مصفوفة أرقام الصفحات لتوليد المعاينات.


**Returns:**
int[] - مجموعة من أرقام الصفحات.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


يضبط مصفوفة أرقام الصفحات لتوليد المعاينات.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | pageNumbers | int[] | مجموعة من أرقام الصفحات. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


يحصل على تنسيق صورة المعاينة.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


يضبط تنسيق صورة المعاينة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | تنسيق المعاينة. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


يحصل على نسخة من المندوب لإنشاء تدفق الصفحة.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


يضبط نسخة من المندوب لإنشاء تدفق الصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | المندوب الخاص بإنشاء تدفق الصفحة. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


يحصل على نسخة من المندوب لإكمال معاينة الصفحة.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


يضبط نسخة من المندوب لإكمال معاينة الصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | المندوب الخاص بإكمال معاينة الصفحة. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


يحصل على نسخة من المندوب لمعلومات عرض معاينة الصفحة.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


يضبط نسخة من المندوب لمعلومات عرض معاينة الصفحة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | المندوب الخاص بمعلومات عرض معاينة الصفحة. |
|

