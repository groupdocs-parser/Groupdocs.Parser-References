---
title: "ImageOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för bildutvinning."
type: docs
weight: 23
url: /sv/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Tillhandahåller de alternativ som används för bildutvinning.

En instans av klassen [ImageOptions](../../com.groupdocs.parser.options/imageoptions) används som parameter
i [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) och
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Den används för att ange bildformatet för bildextraktion.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Tillhandahåller de alternativ som används för bildutvinning. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Hämtar bildformatet för bildextraktion. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Tillhandahåller de alternativ som används för bildutvinning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Formatet för bilden. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Hämtar bildformatet för bildextraktion.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

