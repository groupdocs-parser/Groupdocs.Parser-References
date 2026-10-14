---
title: "PageImageArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablonla ayrıştırma işlevinde sayfada bir resmi temsil etmek veya e-postalardan veya Zip arşivlerinden çıkarılan resimler için bir resim eki temsil etmek amacıyla kullanılan bir sayfa resim alanını temsil eder."
type: docs
weight: 21
url: /tr/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Şablonla ayrıştırma işlevinde sayfada bir resmi temsil etmek veya e-postalardan veya Zip arşivlerinden çıkarılan resimler için bir resim eki temsil etmek amacıyla kullanılan bir sayfa resim alanını temsil eder.

Bir [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) sınıfının örneği aşağıdaki yöntemlerin dönüş değeri olarak kullanılır:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Oradaki kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Yeni bir [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) sınıfının örneğini başlatır. |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Yeni bir [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileType()](#getFileType--) | Görselin biçimini alır. |
|
|  | [getRotation()](#getRotation--) | Görselin döndürme açısını alır. |
|
|  | [getImageStream()](#getImageStream--) | Görsel akışını döndürür. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Görsel akışını farklı bir biçimde döndürür. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Görseli dosyaya kaydeder. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Görseli farklı bir biçimde dosyaya kaydeder. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Yeni bir [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Görselin akışı. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Görüntünün formatı. |
|
|  | rotasyon | double | Görselin döndürme açısı. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Yeni bir [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Görselin akışı. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Görüntünün formatı. |
|
|  | rotasyon | double | Görselin döndürme açısı. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Görseli içeren sayfa. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Görseli içeren dikdörtgen alan. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Görselin biçimini alır.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Görselin döndürme açısını alır.


**Returns:**
double - Görselin döndürme açısını temsil eden çift değer.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Görsel akışını döndürür.

Aşağıdaki örnek, görselleri dosyalara nasıl kaydedeceğinizi gösterir:

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
java.io.InputStream - Görsel içeren bir akış.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Görsel akışını farklı bir biçimde döndürür.

Aşağıdaki örnek, görselleri PNG biçiminde nasıl kaydedeceğinizi gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Görseli çıkarmak için kullanılan seçenekler. |
|

**Returns:**
java.io.InputStream - Görsel içeren bir akış

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Görseli dosyaya kaydeder.

Aşağıdaki örnek, görselleri dosyalara nasıl kaydedeceğinizi gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Görseli farklı bir biçimde dosyaya kaydeder.

Aşağıdaki örnek, görselleri PNG biçiminde dosyalara nasıl kaydedeceğinizi gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosyanın yolu. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Görseli kaydetmek için kullanılan seçenekler. |
|

