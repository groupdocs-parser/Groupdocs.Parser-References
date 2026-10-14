---
title: "ImageOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "इमेज निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 23
url: /hi/java/com.groupdocs.parser.options/imageoptions/
---
**Inheritance:**
java.lang.Object
```
public final class ImageOptions
```

इमेज निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

[ImageOptions](../../com.groupdocs.parser.options/imageoptions) क्लास का एक उदाहरण पैरामीटर के रूप में उपयोग किया जाता है।
में [PageImageArea.getImageStream(ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#getImageStream-ImageOptions-) और
[PageImageArea.save(String, ImageOptions)](../../com.groupdocs.parser.data/pageimagearea#save-String--ImageOptions-) methods. See the usage examples there.

इसे इमेज एक्सट्रैक्शन के लिए इमेज फ़ॉर्मेट निर्दिष्ट करने हेतु उपयोग किया जाता है।

**Learn more:**

* [Extract images from document page area](../https://docs.groupdocs.com/display/parserjava/Extract+images+from+document+page+area)
* [Extract images to files](../https://docs.groupdocs.com/display/parserjava/Extract+images+to+files)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [ImageOptions(ImageFormat imageFormat)](#ImageOptions-com.groupdocs.parser.options.ImageFormat-) | इमेज निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getImageFormat()](#getImageFormat--) | इमेज एक्सट्रैक्शन के लिए इमेज फ़ॉर्मेट प्राप्त करता है। |
|
### ImageOptions(ImageFormat imageFormat) {#ImageOptions-com.groupdocs.parser.options.ImageFormat-}
```
public ImageOptions(ImageFormat imageFormat)
```


इमेज निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageFormat | [ImageFormat](../../com.groupdocs.parser.options/imageformat) | छवि का प्रारूप। |
|

### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


इमेज एक्सट्रैक्शन के लिए इमेज फ़ॉर्मेट प्राप्त करता है।


**Returns:**
[ImageFormat](../../com.groupdocs.parser.options/imageformat) - [ImageFormat](../../com.groupdocs.parser.options/imageformat) enumeration that contains an image format.

