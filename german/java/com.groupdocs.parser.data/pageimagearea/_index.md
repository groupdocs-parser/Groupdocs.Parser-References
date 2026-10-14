---
title: "PageImageArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Seiten‑Bild‑Bereich dar, der verwendet wird, um ein Bild auf der Seite in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren oder einen Bildanhang, wenn Bilder aus E‑Mails oder Zip‑Archiven extrahiert werden."
type: docs
weight: 21
url: /de/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Stellt einen Seiten‑Bild‑Bereich dar, der verwendet wird, um ein Bild auf der Seite in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren oder einen Bildanhang, wenn Bilder aus E‑Mails oder Zip‑Archiven extrahiert werden.

Eine Instanz der Klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) wird als Rückgabewert der folgenden Methoden verwendet:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Initialisiert eine neue Instanz der Klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFileType()](#getFileType--) | Liefert das Format des Bildes. |
|
|  | [getRotation()](#getRotation--) | Liefert den Rotationswinkel des Bildes. |
|
|  | [getImageStream()](#getImageStream--) | Gibt den Bild-Stream zurück. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Gibt den Bild-Stream in einem anderen Format zurück. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Speichert das Bild in die Datei. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Speichert das Bild in die Datei in einem anderen Format. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Initialisiert eine neue Instanz der Klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Der Stream des Bildes. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Das Format des Bildes. |
|
|  | rotation | double | Der Rotationswinkel des Bildes. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Der Stream des Bildes. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Das Format des Bildes. |
|
|  | rotation | double | Der Rotationswinkel des Bildes. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die das Bild enthält. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Bild enthält. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Liefert das Format des Bildes.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Liefert den Rotationswinkel des Bildes.


**Returns:**
double - Ein double-Wert, der den Rotationswinkel des Bildes darstellt.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Gibt den Bild-Stream zurück.

Das folgende Beispiel zeigt, wie Bilder in Dateien gespeichert werden:

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
java.io.InputStream - Ein Stream mit dem Bild.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Gibt den Bild-Stream in einem anderen Format zurück.

Das folgende Beispiel zeigt, wie man Bilder im PNG-Format speichert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Die Optionen, die zum Extrahieren des Bildes verwendet werden. |
|

**Returns:**
java.io.InputStream - Ein Stream mit dem Bild

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Speichert das Bild in die Datei.

Das folgende Beispiel zeigt, wie Bilder in Dateien gespeichert werden:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Speichert das Bild in die Datei in einem anderen Format.

Das folgende Beispiel zeigt, wie man Bilder in Dateien im PNG-Format speichert:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Datei. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Die Optionen, die zum Speichern des Bildes verwendet werden. |
|

