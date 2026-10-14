---
title: "ImageOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή εικόνων."
type: docs
weight: 23
url: /el/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή εικόνων.

Μια παρουσία της κλάσης [ImageOptions](../../com.groupdocs.parser.options/imageoptions) χρησιμοποιείται ως παράμετρος
στο [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) και
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Χρησιμοποιείται για να καθορίσει τη μορφή εικόνας για την εξαγωγή εικόνας.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή εικόνων. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Λαμβάνει τη μορφή εικόνας για την εξαγωγή εικόνας. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή εικόνων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Η μορφή της εικόνας. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Λαμβάνει τη μορφή εικόνας για την εξαγωγή εικόνας.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

