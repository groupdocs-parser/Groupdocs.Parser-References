---
title: "ImageOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для извлечения изображений."
type: docs
weight: 23
url: /ru/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Предоставляет параметры, используемые для извлечения изображений.

Экземпляр класса [ImageOptions](../../com.groupdocs.parser.options/imageoptions) используется в качестве параметра.
в [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) и
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Он используется для указания формата изображения при извлечении изображения.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Предоставляет параметры, используемые для извлечения изображений. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Получает формат изображения для извлечения изображения. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Предоставляет параметры, используемые для извлечения изображений.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Формат изображения. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Получает формат изображения для извлечения изображения.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

