---
title: "PageImageArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili area gambar halaman yang digunakan untuk mewakili gambar pada halaman dalam fungsi parsing dengan templat atau lampiran gambar jika gambar diekstrak dari email atau arsip Zip."
type: docs
weight: 21
url: /id/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Mewakili area gambar halaman yang digunakan untuk mewakili gambar pada halaman dalam fungsi parsing dengan templat atau lampiran gambar jika gambar diekstrak dari email atau arsip Zip.

Sebuah instance dari kelas [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) digunakan sebagai nilai kembali dari metode-metode berikut:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Menginisialisasi instance baru dari kelas [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi instance baru dari kelas [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileType()](#getFileType--) | Mendapatkan format gambar. |
|
|  | [getRotation()](#getRotation--) | Mendapatkan sudut rotasi gambar. |
|
|  | [getImageStream()](#getImageStream--) | Mengembalikan aliran gambar. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Mengembalikan aliran gambar dalam format yang berbeda. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Menyimpan gambar ke file. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Menyimpan gambar ke file dalam format yang berbeda. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Menginisialisasi instance baru dari kelas [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Aliran gambar. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Format gambar. |
|
|  | rotasi | double | Sudut rotasi gambar. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Menginisialisasi instance baru dari kelas [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Aliran gambar. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Format gambar. |
|
|  | rotasi | double | Sudut rotasi gambar. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi gambar. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi gambar. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Mendapatkan format gambar.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Mendapatkan sudut rotasi gambar.


**Returns:**
double - Nilai double yang mewakili sudut rotasi gambar.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Mengembalikan aliran gambar.

Contoh berikut menunjukkan cara menyimpan gambar ke file:

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
java.io.InputStream - Aliran dengan gambar.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Mengembalikan aliran gambar dalam format yang berbeda.

Contoh berikut menunjukkan cara menyimpan gambar dalam format PNG:

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Opsi yang digunakan untuk mengekstrak gambar. |
|

**Returns:**
java.io.InputStream - Aliran dengan gambar

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Menyimpan gambar ke file.

Contoh berikut menunjukkan cara menyimpan gambar ke file:

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Menyimpan gambar ke file dalam format yang berbeda.

Contoh berikut menunjukkan cara menyimpan gambar ke file dalam format PNG:

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Opsi yang digunakan untuk menyimpan gambar. |
|

