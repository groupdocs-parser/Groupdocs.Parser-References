---
title: "ImageOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction d'images."
type: docs
weight: 23
url: /fr/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Fournit les options utilisées pour l'extraction d'images.

Une instance de la classe [ImageOptions](../../com.groupdocs.parser.options/imageoptions) est utilisée comme paramètre
dans [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) et
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Il est utilisé pour spécifier le format d'image pour l'extraction d'images.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Fournit les options utilisées pour l'extraction d'images. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Obtient le format d'image pour l'extraction d'images. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Fournit les options utilisées pour l'extraction d'images.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Le format de l'image. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Obtient le format d'image pour l'extraction d'images.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

