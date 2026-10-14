---
title: "PageImageArea"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "템플릿 기반 파싱 기능에서 페이지의 이미지를 나타내는 페이지 이미지 영역 또는 이메일이나 Zip 아카이브에서 추출된 이미지인 경우 이미지 첨부 파일을 나타냅니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

템플릿 기반 파싱 기능에서 페이지의 이미지를 나타내는 페이지 이미지 영역 또는 이메일이나 Zip 아카이브에서 추출된 이미지인 경우 이미지 첨부 파일을 나타냅니다.

다음 메서드들의 반환값으로 [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 클래스의 인스턴스가 사용됩니다:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

그곳의 사용 예제를 확인하십시오.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileType()](#getFileType--) | 이미지의 형식을 가져옵니다. |
|
|  | [getRotation()](#getRotation--) | 이미지의 회전 각도를 가져옵니다. |
|
|  | [getImageStream()](#getImageStream--) | 이미지 스트림을 반환합니다. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | 다른 형식으로 이미지 스트림을 반환합니다. |
|
|  | [save(String filePath)](#save-java.lang.String-) | 이미지를 파일에 저장합니다. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | 이미지를 다른 형식으로 파일에 저장합니다. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


[PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 이미지 스트림. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 이미지의 형식입니다. |
|
|  | 회전 | double | 이미지의 회전 각도. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


[PageImageArea](../../com.groupdocs.parser.data/pageimagearea) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 이미지 스트림. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | 이미지의 형식입니다. |
|
|  | 회전 | double | 이미지의 회전 각도. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 이미지를 포함하는 페이지. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 이미지를 포함하는 사각형 영역. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


이미지의 형식을 가져옵니다.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


이미지의 회전 각도를 가져옵니다.


**Returns:**
double - 이미지의 회전 각도를 나타내는 double 값.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


이미지 스트림을 반환합니다.

다음 예제는 이미지를 파일에 저장하는 방법을 보여줍니다:

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
java.io.InputStream - 이미지가 포함된 스트림.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


다른 형식으로 이미지 스트림을 반환합니다.

다음 예제는 PNG 형식으로 이미지를 저장하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | 이미지를 추출하는 데 사용되는 옵션입니다. |
|

**Returns:**
java.io.InputStream - 이미지를 포함하는 스트림

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


이미지를 파일에 저장합니다.

다음 예제는 이미지를 파일에 저장하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


이미지를 다른 형식으로 파일에 저장합니다.

다음 예제는 PNG 형식으로 이미지를 파일에 저장하는 방법을 보여줍니다:

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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로입니다. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | 이미지를 저장하는 데 사용되는 옵션입니다. |
|

