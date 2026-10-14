---
title: "PageImageArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une zone d'image de page utilisée pour représenter une image sur la page dans la fonctionnalité d'analyse par modèle ou une pièce jointe d'image si les images sont extraites d'e-mails ou d'archives Zip."
type: docs
weight: 21
url: /fr/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Représente une zone d'image de page utilisée pour représenter une image sur la page dans la fonctionnalité d'analyse par modèle ou une pièce jointe d'image si les images sont extraites d'e-mails ou d'archives Zip.

Une instance de la classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) est utilisée comme valeur de retour des méthodes suivantes:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Voir les exemples d'utilisation là-bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Initialise une nouvelle instance de la classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtient le format de l'image. |
|
|  | [getRotation()](#getRotation--) | Obtient l'angle de rotation de l'image. |
|
|  | [getImageStream()](#getImageStream--) | Renvoie le flux de l'image. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Renvoie le flux de l'image dans un format différent. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Enregistre l'image dans le fichier. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Enregistre l'image dans le fichier dans un format différent. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Initialise une nouvelle instance de la classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Le flux de l'image. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Le format de l'image. |
|
|  | rotation | double | L'angle de rotation de l'image. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Le flux de l'image. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Le format de l'image. |
|
|  | rotation | double | L'angle de rotation de l'image. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient l'image. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient l'image. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Obtient le format de l'image.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Obtient l'angle de rotation de l'image.


**Returns:**
double - Une valeur double qui représente l'angle de rotation de l'image.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Renvoie le flux de l'image.

L'exemple suivant montre comment enregistrer des images dans des fichiers:

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
java.io.InputStream - Un flux contenant l'image.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Renvoie le flux de l'image dans un format différent.

L'exemple suivant montre comment enregistrer des images au format PNG:

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Les options utilisées pour extraire l'image. |
|

**Returns:**
java.io.InputStream - Un flux contenant l'image

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Enregistre l'image dans le fichier.

L'exemple suivant montre comment enregistrer des images dans des fichiers:

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Enregistre l'image dans le fichier dans un format différent.

L'exemple suivant montre comment enregistrer des images dans des fichiers au format PNG:

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Les options utilisées pour enregistrer l'image. |
|

