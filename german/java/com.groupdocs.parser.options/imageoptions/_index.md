---
title: "ImageOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Bildextraktion verwendet werden."
type: docs
weight: 23
url: /de/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Stellt die Optionen bereit, die für die Bildextraktion verwendet werden.

Eine Instanz der [ImageOptions](../../com.groupdocs.parser.options/imageoptions)-Klasse wird als Parameter verwendet.
in [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) und
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Sie wird verwendet, um das Bildformat für die Bildextraktion festzulegen.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Stellt die Optionen bereit, die für die Bildextraktion verwendet werden. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Ermittelt das Bildformat für die Bildextraktion. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Stellt die Optionen bereit, die für die Bildextraktion verwendet werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Das Format des Bildes. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Ermittelt das Bildformat für die Bildextraktion.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

