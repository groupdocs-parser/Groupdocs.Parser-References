---
title: "PageImageArea"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'area immagine della pagina che è usata per rappresentare un'immagine nella pagina nella funzionalità di parsing tramite modello o un allegato immagine se le immagini sono estratte da email o archivi Zip."
type: docs
weight: 21
url: /it/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Rappresenta un'area immagine della pagina che è usata per rappresentare un'immagine nella pagina nella funzionalità di parsing tramite modello o un allegato immagine se le immagini sono estratte da email o archivi Zip.

Un'istanza della classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) è utilizzata come valore di ritorno dei seguenti metodi:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Vedi gli esempi di utilizzo lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Inizializza una nuova istanza della classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inizializza una nuova istanza della classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFileType()](#getFileType--) | Restituisce il formato dell'immagine. |
|
|  | [getRotation()](#getRotation--) | Restituisce l'angolo di rotazione dell'immagine. |
|
|  | [getImageStream()](#getImageStream--) | Restituisce lo stream dell'immagine. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Restituisce lo stream dell'immagine in un formato diverso. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Salva l'immagine nel file. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Salva l'immagine nel file in un formato diverso. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Inizializza una nuova istanza della classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Lo stream dell'immagine. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Il formato dell'immagine. |
|
|  | rotazione | double | L'angolo di rotazione dell'immagine. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Inizializza una nuova istanza della classe [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Lo stream dell'immagine. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Il formato dell'immagine. |
|
|  | rotazione | double | L'angolo di rotazione dell'immagine. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La pagina che contiene l'immagine. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene l'immagine. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Restituisce il formato dell'immagine.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Restituisce l'angolo di rotazione dell'immagine.


**Returns:**
double - Un valore double che rappresenta l'angolo di rotazione dell'immagine.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Restituisce lo stream dell'immagine.

Il seguente esempio mostra come salvare le immagini su file:

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
java.io.InputStream - Uno stream con l'immagine.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Restituisce lo stream dell'immagine in un formato diverso.

Il seguente esempio mostra come salvare le immagini in formato PNG:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Le opzioni utilizzate per estrarre l'immagine. |
|

**Returns:**
java.io.InputStream - Uno stream con l'immagine

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Salva l'immagine nel file.

Il seguente esempio mostra come salvare le immagini su file:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Salva l'immagine nel file in un formato diverso.

Il seguente esempio mostra come salvare le immagini su file in formato PNG:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Le opzioni utilizzate per salvare l'immagine. |
|

