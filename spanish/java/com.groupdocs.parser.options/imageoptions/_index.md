---
title: "ImageOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de imágenes."
type: docs
weight: 23
url: /es/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Proporciona las opciones que se utilizan para la extracción de imágenes.

Una instancia de la clase [ImageOptions](../../com.groupdocs.parser.options/imageoptions) se utiliza como parámetro
en [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) y
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Se utiliza para especificar el formato de imagen para la extracción de imágenes.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Proporciona las opciones que se utilizan para la extracción de imágenes. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Obtiene el formato de imagen para la extracción de imágenes. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Proporciona las opciones que se utilizan para la extracción de imágenes.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | El formato de la imagen. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Obtiene el formato de imagen para la extracción de imágenes.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

