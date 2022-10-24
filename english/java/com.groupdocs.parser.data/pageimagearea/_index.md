---
title: PageImageArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents a page image area which is used to represent an image on the page in the parsing by template functionality or an image attachment if images are extracted from emails or Zip archives.
type: docs
weight: 20
url: /java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Represents a page image area which is used to represent an image on the page in the parsing by template functionality or an image attachment if images are extracted from emails or Zip archives.

An instance of [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) class is used as return value of the following methods:

 *  [Parser.getImages()](../../com.groupdocs.parser/parser\#getImages--)
 *  [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser\#getImages-PageAreaOptions-)
 *  [Parser.getImages(int)](../../com.groupdocs.parser/parser\#getImages-int-)
 *  [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser\#getImages-int--PageAreaOptions-)

See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Initializes a new instance of the [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) class. |
| [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) class. |
## Methods

| Method | Description |
| --- | --- |
| [getFileType()](#getFileType--) | Gets the format of the image. |
| [getRotation()](#getRotation--) | Gets the rotation angle of the image. |
| [getImageStream()](#getImageStream--) | Returns the image stream. |
| [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Returns the image stream in a different format. |
| [save(String filePath)](#save-java.lang.String-) | Saves the image to the file. |
| [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Saves the image to the file in a different format. |
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Initializes a new instance of the [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The stream of the image. |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) | The format of the image. |
| rotation | double | The rotation angle of the image. |

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Initializes a new instance of the [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The stream of the image. |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) | The format of the image. |
| rotation | double | The rotation angle of the image. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the image. |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the image. |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Gets the format of the image.

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.
### getRotation() {#getRotation--}
```
public double getRotation()
```


Gets the rotation angle of the image.

**Returns:**
double - A double value that represents the rotation angle of the image.
### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Returns the image stream.

The following example shows how to save images to files:

```
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
 
```

**Returns:**
java.io.InputStream - A stream with the image.
### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Returns the image stream in a different format.

The following example shows how to save images in PNG format:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | The options which are used to extract the image. |

**Returns:**
java.io.InputStream - A stream with the image
### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Saves the image to the file.

The following example shows how to save images to files:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The path to the file. |

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Saves the image to the file in a different format.

The following example shows how to save images to files in PNG format:

```
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
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The path to the file. |
| options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | The options which are used to save the image. |

