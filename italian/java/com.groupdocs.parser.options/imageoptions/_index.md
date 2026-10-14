---
title: "ImageOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione di immagini."
type: docs
weight: 23
url: /it/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

Fornisce le opzioni utilizzate per l'estrazione di immagini.

Un'istanza della classe [ImageOptions](../../com.groupdocs.parser.options/imageoptions) è utilizzata come parametro
in [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) e
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

Viene utilizzato per specificare il formato dell'immagine per l'estrazione dell'immagine.

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | Fornisce le opzioni utilizzate per l'estrazione di immagini. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | Restituisce il formato dell'immagine per l'estrazione dell'immagine. |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


Fornisce le opzioni utilizzate per l'estrazione di immagini.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | Il formato dell'immagine. |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


Restituisce il formato dell'immagine per l'estrazione dell'immagine.


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

