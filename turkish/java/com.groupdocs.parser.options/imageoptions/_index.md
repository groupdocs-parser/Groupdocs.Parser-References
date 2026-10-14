---
title: "ImageOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Görüntü çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 23
url: /tr/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Görüntü çıkarımı için kullanılan seçenekleri sağlar.

Bir parametre olarak kullanılan [ImageOptions](../../com.groupdocs.parser.options/imageoptions) sınıfının bir örneği
içinde [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) ve
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Görüntü çıkarma için görüntü formatını belirtmekte kullanılır.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Görüntü çıkarımı için kullanılan seçenekleri sağlar. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Görüntü çıkarma için görüntü formatını alır. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Görüntü çıkarımı için kullanılan seçenekleri sağlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Görüntünün formatı. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Görüntü çıkarma için görüntü formatını alır.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

