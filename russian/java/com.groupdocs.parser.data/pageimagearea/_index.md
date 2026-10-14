---
title: "PageImageArea"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет область изображения на странице, которая используется для представления изображения на странице в функции разбора по шаблону или вложения изображения, если изображения извлекаются из электронных писем или Zip‑архивов."
type: docs
weight: 21
url: /ru/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Представляет область изображения на странице, которая используется для представления изображения на странице в функции разбора по шаблону или вложения изображения, если изображения извлекаются из электронных писем или Zip‑архивов.

Экземпляр класса [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) используется в качестве возвращаемого значения следующих методов:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Смотрите примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Инициализирует новый экземпляр класса [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Инициализирует новый экземпляр класса [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFileType()](#getFileType--) | Получает формат изображения. |
|
|  | [getRotation()](#getRotation--) | Получает угол поворота изображения. |
|
|  | [getImageStream()](#getImageStream--) | Возвращает поток изображения. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Возвращает поток изображения в другом формате. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Сохраняет изображение в файл. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Сохраняет изображение в файл в другом формате. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Инициализирует новый экземпляр класса [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Поток изображения. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Формат изображения. |
|
|  | вращение | double | Угол вращения изображения. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Инициализирует новый экземпляр класса [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Поток изображения. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Формат изображения. |
|
|  | вращение | double | Угол вращения изображения. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Страница, содержащая изображение. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Прямоугольная область, содержащая изображение. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Получает формат изображения.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Получает угол поворота изображения.


**Returns:**
double - значение типа double, представляющее угол вращения изображения.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Возвращает поток изображения.

В следующем примере показано, как сохранять изображения в файлы:

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
java.io.InputStream - поток с изображением.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Возвращает поток изображения в другом формате.

В следующем примере показано, как сохранять изображения в формате PNG:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Параметры, используемые для извлечения изображения. |
|

**Returns:**
java.io.InputStream - поток с изображением

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Сохраняет изображение в файл.

В следующем примере показано, как сохранять изображения в файлы:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Сохраняет изображение в файл в другом формате.

В следующем примере показано, как сохранять изображения в файлы в формате PNG:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Параметры, используемые для сохранения изображения. |
|

