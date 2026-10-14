---
title: "PageImageArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un área de imagen de página que se utiliza para representar una imagen en la página en la funcionalidad de análisis mediante plantillas o un adjunto de imagen si las imágenes se extraen de correos electrónicos o archivos Zip."
type: docs
weight: 21
url: /es/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Representa un área de imagen de página que se utiliza para representar una imagen en la página en la funcionalidad de análisis mediante plantillas o un adjunto de imagen si las imágenes se extraen de correos electrónicos o archivos Zip.

Una instancia de la clase [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) se usa como valor de retorno de los siguientes métodos:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Vea los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Inicializa una nueva instancia de la clase [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFileType()](#getFileType--) | Obtiene el formato de la imagen. |
|
|  | [getRotation()](#getRotation--) | Obtiene el ángulo de rotación de la imagen. |
|
|  | [getImageStream()](#getImageStream--) | Devuelve el flujo de la imagen. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Devuelve el flujo de la imagen en un formato diferente. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Guarda la imagen en el archivo. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Guarda la imagen en el archivo en un formato diferente. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Inicializa una nueva instancia de la clase [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | El flujo de la imagen. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | El formato de la imagen. |
|
|  | rotación | double | El ángulo de rotación de la imagen. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | El flujo de la imagen. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | El formato de la imagen. |
|
|  | rotación | double | El ángulo de rotación de la imagen. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene la imagen. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene la imagen. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Obtiene el formato de la imagen.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Obtiene el ángulo de rotación de la imagen.


**Returns:**
double - Un valor double que representa el ángulo de rotación de la imagen.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Devuelve el flujo de la imagen.

El siguiente ejemplo muestra cómo guardar imágenes en archivos:

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
java.io.InputStream - Un flujo con la imagen.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Devuelve el flujo de la imagen en un formato diferente.

El siguiente ejemplo muestra cómo guardar imágenes en formato PNG:

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Las opciones que se utilizan para extraer la imagen. |
|

**Returns:**
java.io.InputStream - Un flujo con la imagen

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Guarda la imagen en el archivo.

El siguiente ejemplo muestra cómo guardar imágenes en archivos:

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta al archivo. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Guarda la imagen en el archivo en un formato diferente.

El siguiente ejemplo muestra cómo guardar imágenes en archivos en formato PNG:

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta al archivo. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Las opciones que se utilizan para guardar la imagen. |
|

