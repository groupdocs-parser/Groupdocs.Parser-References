---
title: "PageImageArea"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在基于模板的解析功能中表示页面图像的页面图像区域，或在从电子邮件或 Zip 存档中提取图像时表示图像附件。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

表示用于在基于模板的解析功能中表示页面图像的页面图像区域，或在从电子邮件或 Zip 存档中提取图像时表示图像附件。

以下方法的返回值使用 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 类的实例：

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | 初始化 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 类的新实例。 |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 初始化 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 获取图像的格式。 |
|
|  | [getRotation()](#getRotation--) | 获取图像的旋转角度。 |
|
|  | [getImageStream()](#getImageStream--) | 返回图像流。 |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | 以不同的格式返回图像流。 |
|
|  | [save(String filePath)](#save-java.lang.String-) | 将图像保存到文件。 |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | 以不同的格式将图像保存到文件。 |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


初始化 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 图像的流。 |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 图像的格式。 |
|
|  | 旋转 | double | 图像的旋转角度。 |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


初始化 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 图像的流。 |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 图像的格式。 |
|
|  | 旋转 | double | 图像的旋转角度。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含图像的页面。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含图像的矩形区域。 |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


获取图像的格式。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


获取图像的旋转角度。


**Returns:**
double - 表示图像旋转角度的 double 值。

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


返回图像流。

下面的示例展示了如何将图像保存到文件：

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
java.io.InputStream - 包含图像的流。

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


以不同的格式返回图像流。

以下示例展示了如何以 PNG 格式保存图像：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | 用于提取图像的选项。 |
|

**Returns:**
java.io.InputStream - 包含图像的流

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


将图像保存到文件。

下面的示例展示了如何将图像保存到文件：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


以不同的格式将图像保存到文件。

以下示例展示了如何以 PNG 格式将图像保存到文件：

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件的路径。 |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | 用于保存图像的选项。 |
|

