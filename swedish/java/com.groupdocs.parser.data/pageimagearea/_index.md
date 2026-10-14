---
title: "PageImageArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett sidområde för bild som används för att representera en bild på sidan i funktionaliteten för parsning med mall eller en bildbilaga om bilder extraheras från e‑post eller Zip‑arkiv."
type: docs
weight: 21
url: /sv/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Representerar ett sidområde för bild som används för att representera en bild på sidan i funktionaliteten för parsning med mall eller en bildbilaga om bilder extraheras från e‑post eller Zip‑arkiv.

En instans av klassen [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) används som returvärde för följande metoder:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Initierar en ny instans av klassen [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFileType()](#getFileType--) | Hämtar bildens format. |
|
|  | [getRotation()](#getRotation--) | Hämtar bildens rotationsvinkel. |
|
|  | [getImageStream()](#getImageStream--) | Returnerar bildströmmen. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Returnerar bildströmmen i ett annat format. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Sparar bilden till filen. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Sparar bilden till filen i ett annat format. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Initierar en ny instans av klassen [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Strömmen för bilden. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Formatet för bilden. |
|
|  | rotation | double | Rotationsvinkeln för bilden. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Strömmen för bilden. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Formatet för bilden. |
|
|  | rotation | double | Rotationsvinkeln för bilden. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller bilden. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller bilden. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Hämtar bildens format.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Hämtar bildens rotationsvinkel.


**Returns:**
double - Ett dubbelvärde som representerar bildens rotationsvinkel.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Returnerar bildströmmen.

Följande exempel visar hur man sparar bilder till filer:

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
java.io.InputStream - En ström med bilden.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Returnerar bildströmmen i ett annat format.

Följande exempel visar hur man sparar bilder i PNG-format:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Alternativen som används för att extrahera bilden. |
|

**Returns:**
java.io InputStream - En ström med bilden

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Sparar bilden till filen.

Följande exempel visar hur man sparar bilder till filer:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Sparar bilden till filen i ett annat format.

Följande exempel visar hur man sparar bilder till filer i PNG-format:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till filen. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Alternativen som används för att spara bilden. |
|

