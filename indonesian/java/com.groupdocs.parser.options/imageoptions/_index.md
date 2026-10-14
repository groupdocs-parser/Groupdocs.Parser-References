---
title: "ImageOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi gambar."
type: docs
weight: 23
url: /id/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi gambar.

Sebuah instance dari kelas [ImageOptions](../../com.groupdocs.parser.options/imageoptions) digunakan sebagai parameter
di [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) dan
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Ini digunakan untuk menentukan format gambar untuk ekstraksi gambar.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Menyediakan opsi yang digunakan untuk ekstraksi gambar. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Mendapatkan format gambar untuk ekstraksi gambar. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Menyediakan opsi yang digunakan untuk ekstraksi gambar.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Format gambar. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Mendapatkan format gambar untuk ekstraksi gambar.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

