---
title: "PageImageArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل منطقة صورة الصفحة التي تُستخدم لتمثيل صورة على الصفحة في وظيفة التحليل باستخدام القالب أو مرفق صورة إذا تم استخراج الصور من رسائل البريد الإلكتروني أو أرشيفات Zip."
type: docs
weight: 21
url: /ar/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object، [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

يمثل منطقة صورة الصفحة التي تُستخدم لتمثيل صورة على الصفحة في وظيفة التحليل باستخدام القالب أو مرفق صورة إذا تم استخراج الصور من رسائل البريد الإلكتروني أو أرشيفات Zip.

يتم استخدام مثيل من الفئة [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) كقيمة إرجاع للطرق التالية:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

انظر أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | ينشئ مثيلاً جديداً من الفئة [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | ينشئ مثيلاً جديداً من الفئة [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getFileType()](#getFileType--) | يحصل على تنسيق الصورة. |
|
|  | [getRotation()](#getRotation--) | يحصل على زاوية دوران الصورة. |
|
|  | [getImageStream()](#getImageStream--) | يعيد تدفق الصورة. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | يعيد تدفق الصورة بتنسيق مختلف. |
|
|  | [save(String filePath)](#save-java.lang.String-) | يحفظ الصورة إلى الملف. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | يحفظ الصورة إلى الملف بتنسيق مختلف. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


ينشئ مثيلاً جديداً من الفئة [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | تدفق الصورة. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | تنسيق الصورة. |
|
|  | دوران | double | زاوية دوران الصورة. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


ينشئ مثيلاً جديداً من الفئة [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | تدفق الصورة. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | تنسيق الصورة. |
|
|  | دوران | double | زاوية دوران الصورة. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | الصفحة التي تحتوي على الصورة. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | المنطقة المستطيلة التي تحتوي على الصورة. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


يحصل على تنسيق الصورة.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


يحصل على زاوية دوران الصورة.


**Returns:**
double - قيمة مزدوجة تمثل زاوية دوران الصورة.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


يعيد تدفق الصورة.

المثال التالي يوضح كيفية حفظ الصور إلى ملفات:

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
java.io.InputStream - تدفق يحتوي على الصورة.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


يعيد تدفق الصورة بتنسيق مختلف.

المثال التالي يوضح كيفية حفظ الصور بتنسيق PNG:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | الخيارات المستخدمة لاستخراج الصورة. |
|

**Returns:**
java.io.InputStream - تدفق يحتوي على الصورة

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


يحفظ الصورة إلى الملف.

المثال التالي يوضح كيفية حفظ الصور إلى ملفات:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


يحفظ الصورة إلى الملف بتنسيق مختلف.

المثال التالي يوضح كيفية حفظ الصور إلى ملفات بتنسيق PNG:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | الخيارات المستخدمة لحفظ الصورة. |
|

