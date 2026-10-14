---
title: "ImageOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor het extraheren van afbeeldingen."
type: docs
weight: 23
url: /nl/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Biedt de opties die worden gebruikt voor het extraheren van afbeeldingen.

Een instantie van de [ImageOptions](../../com.groupdocs.parser.options/imageoptions) klasse wordt gebruikt als parameter
in [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) en
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Het wordt gebruikt om het afbeeldingsformaat voor afbeeldingsextractie op te geven.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Biedt de opties die worden gebruikt voor het extraheren van afbeeldingen. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Haalt het afbeeldingsformaat voor afbeeldingsextractie op. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Biedt de opties die worden gebruikt voor het extraheren van afbeeldingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Het formaat van de afbeelding. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Haalt het afbeeldingsformaat voor afbeeldingsextractie op.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

