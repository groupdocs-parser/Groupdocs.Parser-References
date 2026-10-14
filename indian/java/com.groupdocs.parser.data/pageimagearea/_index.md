---
title: "PageImageArea"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में पृष्ठ पर छवि को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ इमेज क्षेत्र या यदि छवियों को ईमेल या ज़िप आर्काइव से निकाला जाता है तो इमेज अटैचमेंट का प्रतिनिधित्व करता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

टेम्प्लेट द्वारा पार्सिंग कार्यक्षमता में पृष्ठ पर छवि को दर्शाने के लिए उपयोग किए जाने वाले पृष्ठ इमेज क्षेत्र या यदि छवियों को ईमेल या ज़िप आर्काइव से निकाला जाता है तो इमेज अटैचमेंट का प्रतिनिधित्व करता है।

[PageImageArea](../../com.groupdocs.parser.data/pageimagearea) क्लास का एक इंस्टेंस निम्नलिखित मेथड्स के रिटर्न वैल्यू के रूप में उपयोग किया जाता है:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

वहाँ उपयोग उदाहरण देखें।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | नए [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | नए [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getFileType()](#getFileType--) | छवि का फॉर्मेट प्राप्त करता है। |
|
|  | [getRotation()](#getRotation--) | छवि का रोटेशन एंगल प्राप्त करता है। |
|
|  | [getImageStream()](#getImageStream--) | छवि स्ट्रीम को लौटाता है। |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | छवि स्ट्रीम को विभिन्न प्रारूप में लौटाता है। |
|
|  | [save(String filePath)](#save-java.lang.String-) | छवि को फ़ाइल में सहेजता है। |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | छवि को विभिन्न प्रारूप में फ़ाइल में सहेजता है। |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


नए [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | छवि की स्ट्रीम। |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | छवि का प्रारूप। |
|
|  | रोटेशन | double | छवि का रोटेशन कोण। |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


नए [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | छवि की स्ट्रीम। |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | छवि का प्रारूप। |
|
|  | रोटेशन | double | छवि का रोटेशन कोण। |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | पृष्ठ जिसमें छवि सम्मिलित है। |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | आयताकार क्षेत्र जिसमें छवि सम्मिलित है। |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


छवि का फॉर्मेट प्राप्त करता है।


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


छवि का रोटेशन एंगल प्राप्त करता है।


**Returns:**
double - एक डबल मान जो छवि के रोटेशन कोण को दर्शाता है।

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


छवि स्ट्रीम को लौटाता है।

निम्नलिखित उदाहरण दिखाता है कि छवियों को फ़ाइलों में कैसे सहेजा जाए:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }
     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images) {
         // Open the image stream
         try (InputStream imageStream = image.getImageStream()) {
             // Create the file to save image
             try (OutputStream destStream = new FileOutputStream(imageNumber + image.getFileType().getExtension())) {
                 byte[] buffer = new byte[4096];
                 int readed = 0;
                 do {
                     // Read data from the image stream
                     readed = imageStream.read(buffer, 0, buffer.length);
                     if (readed > 0) {
                         // Write data to the file stream
                         destStream.write(buffer, 0, readed);
                     }
                 }
                 while (readed > 0);
             }
             imageNumber++;
         }
     }
 }
 
````



**Returns:**
java.io.InputStream - छवि वाली स्ट्रीम।

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


छवि स्ट्रीम को विभिन्न प्रारूप में लौटाता है।

निम्नलिखित उदाहरण दिखाता है कि PNG प्रारूप में छवियों को कैसे सहेजा जाए:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();
     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }

     // Create the options to save images in PNG format
     ImageOptions options = new ImageOptions(ImageFormat.Png);

     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images) {
         // Open the image stream
         try (InputStream imageStream = image.getImageStream(options)) {
             // Create the file to save image
             try (OutputStream destStream = new FileOutputStream(imageNumber + ".png")) {
                 byte[] buffer = new byte[4096];
                 int readed = 0;
                 do {
                     // Read data from the image stream
                     readed = imageStream.read(buffer, 0, buffer.length);
                     if (readed > 0) {
                         // Write data to the file stream
                         destStream.write(buffer, 0, readed);
                     }
                 }
                 while (readed > 0);
             }
             imageNumber++;
         }
     }
 }
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | विकल्प जो छवि निकालने के लिए उपयोग किए जाते हैं। |
|

**Returns:**
java.io.InputStream - छवि वाली स्ट्रीम

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


छवि को फ़ाइल में सहेजता है।

निम्नलिखित उदाहरण दिखाता है कि छवियों को फ़ाइलों में कैसे सहेजा जाए:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();

     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }

     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images)
     {
         // Save the image to the file
         image.save(Constants.getOutputFilePath(String.format("%d", imageNumber) + image.getFileType().getExtension()));

         imageNumber++;
     }
 }
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


छवि को विभिन्न प्रारूप में फ़ाइल में सहेजता है।

निम्नलिखित उदाहरण दिखाता है कि PNG प्रारूप में छवियों को फ़ाइलों में कैसे सहेजा जाए:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleZip)) {
     // Extract images from document
     Iterable images = parser.getImages();

     // Check if images extraction is supported
     if (images == null) {
         System.out.println("Page images extraction isn't supported");
         return;
     }

     // Create the options to save images in PNG format
     ImageOptions options = new ImageOptions(ImageFormat.Png);

     int imageNumber = 0;
     // Iterate over images
     for (PageImageArea image : images)
     {
         // Save the image to the png file
         image.save(Constants.getOutputFilePath(String.format("%d.png", imageNumber)), options);

         imageNumber++;
     }
 }
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | विकल्प जो छवि सहेजने के लिए उपयोग किए जाते हैं। |
|

