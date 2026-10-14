---
title: "PageImageArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια περιοχή εικόνας σελίδας που χρησιμοποιείται για την αναπαράσταση μιας εικόνας στη σελίδα στη λειτουργία ανάλυσης με πρότυπο ή ένα συνημμένο εικόνας εάν οι εικόνες εξάγονται από email ή αρχεία Zip."
type: docs
weight: 21
url: /el/java/com.groupdocs.parser.data/pageimagearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageImageArea extends PageArea
```

Αντιπροσωπεύει μια περιοχή εικόνας σελίδας που χρησιμοποιείται για την αναπαράσταση μιας εικόνας στη σελίδα στη λειτουργία ανάλυσης με πρότυπο ή ένα συνημμένο εικόνας εάν οι εικόνες εξάγονται από email ή αρχεία Zip.

Μία παρουσία της κλάσης [PageImageArea](../../com.groupdocs.parser.data/pageimagearea) χρησιμοποιείται ως τιμή επιστροφής των παρακάτω μεθόδων:

* [Parser.getImages()](../../com.groupdocs.parser/parser#getImages--)
* [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
* [Parser.getImages(int)](../../com.groupdocs.parser/parser#getImages-int-)
* [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-)

Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
|  | [PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)](#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [PageImageArea](../../com.groupdocs.parser.data/pageimagearea). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileType()](#getFileType--) | Λαμβάνει τη μορφή της εικόνας. |
|
|  | [getRotation()](#getRotation--) | Λαμβάνει τη γωνία περιστροφής της εικόνας. |
|
|  | [getImageStream()](#getImageStream--) | Επιστρέφει τη ροή εικόνας. |
|
|  | [getImageStream(ImageOptions options)](#getImageStream-com.groupdocs.parser.options.ImageOptions-) | Επιστρέφει τη ροή εικόνας σε διαφορετική μορφή. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Αποθηκεύει την εικόνα στο αρχείο. |
|
|  | [save(String filePath, ImageOptions options)](#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-) | Αποθηκεύει την εικόνα στο αρχείο σε διαφορετική μορφή. |
|
### PageImageArea(InputStream imageStream, FileType fileType, double rotation) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Η ροή της εικόνας. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Η μορφή της εικόνας. |
|
|  | περιστροφή | double | Η γωνία περιστροφής της εικόνας. |
|

### PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle) {#PageImageArea-java.io.InputStream-com.groupdocs.parser.options.FileType-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageImageArea(InputStream imageStream, FileType fileType, double rotation, Page page, Rectangle rectangle)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [PageImageArea](../../com.groupdocs.parser.data/pageimagearea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Η ροή της εικόνας. |
|
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Η μορφή της εικόνας. |
|
|  | περιστροφή | double | Η γωνία περιστροφής της εικόνας. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει την εικόνα. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει την εικόνα. |
|

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Λαμβάνει τη μορφή της εικόνας.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the format of the image.

### getRotation() {#getRotation--}
```
public double getRotation()
```


Λαμβάνει τη γωνία περιστροφής της εικόνας.


**Returns:**
double - Μια τιμή double που αντιπροσωπεύει τη γωνία περιστροφής της εικόνας.

### getImageStream() {#getImageStream--}
```
public InputStream getImageStream()
```


Επιστρέφει τη ροή εικόνας.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε εικόνες σε αρχεία:

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
java.io.InputStream - Μια ροή με την εικόνα.

### getImageStream(ImageOptions options) {#getImageStream-com.groupdocs.parser.options.ImageOptions-}
```
public InputStream getImageStream(ImageOptions options)
```


Επιστρέφει τη ροή εικόνας σε διαφορετική μορφή.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε εικόνες σε μορφή PNG:

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Οι επιλογές που χρησιμοποιούνται για την εξαγωγή της εικόνας. |
|

**Returns:**
java.io.InputStream - Μια ροή με την εικόνα

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Αποθηκεύει την εικόνα στο αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε εικόνες σε αρχεία:

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|

### save(String filePath, ImageOptions options) {#save-java.lang.String-com.groupdocs.parser.options.ImageOptions-}
```
public void save(String filePath, ImageOptions options)
```


Αποθηκεύει την εικόνα στο αρχείο σε διαφορετική μορφή.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε εικόνες σε αρχεία σε μορφή PNG:

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|
|  | options | [ImageOptions](../../com.groupdocs.parser.options/imageoptions) | Οι επιλογές που χρησιμοποιούνται για την αποθήκευση της εικόνας. |
|

