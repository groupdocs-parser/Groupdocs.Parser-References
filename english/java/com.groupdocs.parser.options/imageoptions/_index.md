---
title: ImageOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for image extraction.
type: docs
weight: 23
url: /java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Provides the options which are used for image extraction.

An instance of [ImageOptions](../../com.groupdocs.parser.options/imageoptions) class is used as parameter in [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea\#getImageStream-ImageOptions-) and [PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea\#save-String--ImageOptions-) methods. See the usage examples there.

It's used to specify the image format for image extraction.

**Learn more:**

 *  [Extract images from document page area][]
 *  [Extract images to files][]


[Extract images from document page area]: https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area
[Extract images to files]: https://docs.groupdocs.com/display/parserjava/Extract+images+to+files
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Provides the options which are used for image extraction. |
## Methods

| Method | Description |
| --- | --- |
| [getImageFormat()](#getImageFormat--) | Gets the image format for image extraction. |
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Provides the options which are used for image extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | The format of the image. |

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Gets the image format for image extraction.

**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.
