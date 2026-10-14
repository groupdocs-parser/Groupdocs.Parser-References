---
title: "ImageOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于图像提取的选项。"
type: docs
weight: 23
url: /zh/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

提供用于图像提取的选项。

使用 [ImageOptions](../../com.groupdocs.parser.options/imageoptions) 类的实例作为参数
在 [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) 中以及
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

用于指定图像提取的图像格式。

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | 提供用于图像提取的选项。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | 获取图像提取的图像格式。 |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


提供用于图像提取的选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | 图像的格式。 |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


获取图像提取的图像格式。


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

