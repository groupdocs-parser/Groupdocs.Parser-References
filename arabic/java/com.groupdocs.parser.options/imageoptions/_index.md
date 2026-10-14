---
title: "ImageOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لاستخراج الصور."
type: docs
weight: 23
url: /ar/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

يوفر الخيارات المستخدمة لاستخراج الصور.

يُستخدم مثيل من فئة [ImageOptions](../../com.groupdocs.parser.options/imageoptions) كمعامل
في [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) و
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

يُستخدم لتحديد تنسيق الصورة لاستخراج الصورة.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | يوفر الخيارات المستخدمة لاستخراج الصور. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | يحصل على تنسيق الصورة لاستخراج الصورة. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


يوفر الخيارات المستخدمة لاستخراج الصور.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | تنسيق الصورة. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


يحصل على تنسيق الصورة لاستخراج الصورة.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

