---
title: "PageImageArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een paginabeeldgebied voor dat wordt gebruikt om een afbeelding op de pagina te representeren in de functionaliteit voor parsing op basis van sjablonen of een afbeeldingbijlage als afbeeldingen worden geëxtraheerd uit e‑mails of Zip‑archieven."
type: docs
weight: 21
url: /nl/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Stelt een paginabeeldgebied voor dat wordt gebruikt om een afbeelding op de pagina te representeren in de functionaliteit voor parsing op basis van sjablonen of een afbeeldingbijlage als afbeeldingen worden geëxtraheerd uit e‑mails of Zip‑archieven.

Een instantie van de klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) wordt gebruikt als retourwaarde van de volgende methoden:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Zie daar de gebruiksvoorbeelden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Initialiseert een nieuw exemplaar van de klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFileType()](#getFileType--) | Haalt het formaat van de afbeelding op. |
|
|  | [getRotation()](#getRotation--) | Haalt de rotatiehoek van de afbeelding op. |
|
|  | [getImageStream()](#getImageStream--) | Retourneert de afbeeldingsstroom. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Retourneert de afbeeldingsstroom in een ander formaat. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Slaat de afbeelding op in het bestand. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Slaat de afbeelding op in het bestand in een ander formaat. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Initialiseert een nieuw exemplaar van de klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | De stroom van de afbeelding. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Het formaat van de afbeelding. |
|
|  | rotatie | double | De rotatiehoek van de afbeelding. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | De stroom van de afbeelding. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Het formaat van de afbeelding. |
|
|  | rotatie | double | De rotatiehoek van de afbeelding. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die de afbeelding bevat. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat de afbeelding bevat. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Haalt het formaat van de afbeelding op.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Haalt de rotatiehoek van de afbeelding op.


**Returns:**
double - Een double-waarde die de rotatiehoek van de afbeelding weergeeft.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Retourneert de afbeeldingsstroom.

Het volgende voorbeeld toont hoe afbeeldingen op te slaan naar bestanden:

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
java.io.InputStream - Een stroom met de afbeelding.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Retourneert de afbeeldingsstroom in een ander formaat.

Het volgende voorbeeld toont hoe afbeeldingen op te slaan in PNG-formaat:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | De opties die worden gebruikt om de afbeelding te extraheren. |
|

**Returns:**
java.io.InputStream - Een stroom met de afbeelding

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Slaat de afbeelding op in het bestand.

Het volgende voorbeeld toont hoe afbeeldingen op te slaan naar bestanden:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Slaat de afbeelding op in het bestand in een ander formaat.

Het volgende voorbeeld toont hoe afbeeldingen op te slaan naar bestanden in PNG-formaat:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het bestand. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | De opties die worden gebruikt om de afbeelding op te slaan. |
|

