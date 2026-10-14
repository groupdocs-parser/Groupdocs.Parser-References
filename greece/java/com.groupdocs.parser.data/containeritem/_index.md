---
title: "ContainerItem"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει ένα στοιχείο κοντέινερ όπως οντότητα αρχείου Zip, συνημμένο email, στοιχείο PDF Portfolio κ.λπ."
type: docs
weight: 10
url: /el/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Αντιπροσωπεύει ένα στοιχείο κοντέινερ όπως οντότητα αρχείου Zip, συνημμένο email, στοιχείο PDF Portfolio κ.λπ.

Μια παρουσία της κλάσης [ContainerItem](../../com.groupdocs.parser.data/containeritem) χρησιμοποιείται ως τιμή επιστροφής της μεθόδου [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--). Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Αρχικοποιεί μια νέα παρουσία της [ContainerItem](../../com.groupdocs.parser.data/containeritem) με το όνομα και τον κατάλογο του στοιχείου. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Αρχικοποιεί μια νέα παρουσία της [ContainerItem](../../com.groupdocs.parser.data/containeritem) με το πλήρες μονοπάτι του στοιχείου. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getName()](#getName--) | Λαμβάνει το όνομα του στοιχείου. |
|
|  | [getDirectory()](#getDirectory--) | Λαμβάνει τον κατάλογο του στοιχείου. |
|
|  | [getFilePath()](#getFilePath--) | Λαμβάνει το πλήρες μονοπάτι του στοιχείου. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το μέγεθος του στοιχείου. |
|
|  | [getMetadata()](#getMetadata--) | Λαμβάνει τη συλλογή των στοιχείων μεταδεδομένων. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Λαμβάνει την τιμή των μεταδεδομένων. |
|
|  | [openStream()](#openStream--) | Ανοίγει τη ροή του περιεχομένου του στοιχείου. |
|
|  | [openParser()](#openParser--) | Δημιουργεί το αντικείμενο [Parser](../../com.groupdocs.parser/parser) για το περιεχόμενο του στοιχείου. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Δημιουργεί το αντικείμενο [Parser](../../com.groupdocs.parser/parser) για το περιεχόμενο του στοιχείου με τις [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Δημιουργεί το αντικείμενο [Parser](../../com.groupdocs.parser/parser) για το περιεχόμενο του στοιχείου με τις [LoadOptions](../../com.groupdocs.parser.options/loadoptions) και τις [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Ανιχνεύει τον τύπο αρχείου του στοιχείου του κοντέινερ. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Αρχικοποιεί μια νέα παρουσία της [ContainerItem](../../com.groupdocs.parser.data/containeritem) με το όνομα και τον κατάλογο του στοιχείου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | όνομα | java.lang.String | Το όνομα του στοιχείου. |
|
|  | κατάλογος | java.lang.String | Ο κατάλογος του στοιχείου. |
|
|  | size | long | Το μέγεθος του στοιχείου. |
|
|  | μεταδεδομένα | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Η συλλογή των στοιχείων μεταδεδομένων. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Αρχικοποιεί μια νέα παρουσία της [ContainerItem](../../com.groupdocs.parser.data/containeritem) με το πλήρες μονοπάτι του στοιχείου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Το πλήρες μονοπάτι του στοιχείου. |
|
|  | size | long | Το μέγεθος του στοιχείου. |
|
|  | μεταδεδομένα | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Η συλλογή των στοιχείων μεταδεδομένων. |
|

### getName() {#getName--}
```
public String getName()
```


Λαμβάνει το όνομα του στοιχείου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το όνομα αρχείου του στοιχείου (χωρίς κατάλογο).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Λαμβάνει τον κατάλογο του στοιχείου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει τον κατάλογο του στοιχείου (χωρίς όνομα αρχείου).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Λαμβάνει το πλήρες μονοπάτι του στοιχείου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το πλήρες μονοπάτι του στοιχείου.

### getSize() {#getSize--}
```
public long getSize()
```


Λαμβάνει το μέγεθος του στοιχείου.


**Returns:**
long - Μια ακέραια τιμή που αντιπροσωπεύει το μέγεθος του στοιχείου σε bytes.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Λαμβάνει τη συλλογή των στοιχείων μεταδεδομένων.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Μια συλλογή από αντικείμενα [MetadataItem](../../com.groupdocs.parser.data/metadataitem); κενή εάν δεν έχουν οριστεί μεταδεδομένα.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Λαμβάνει την τιμή των μεταδεδομένων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | όνομα | java.lang.String | Το όνομα των μεταδεδομένων. |
|

**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει την τιμή του αντικειμένου μεταδεδομένων·  null  εάν δεν βρεθούν μεταδεδομένα με αυτό το όνομα.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Ανοίγει τη ροή του περιεχομένου του στοιχείου.


**Returns:**
java.io.InputStream - Μια ροή με το περιεχόμενο του αντικειμένου.

### openParser() {#openParser--}
```
public Parser openParser()
```


Δημιουργεί το αντικείμενο [Parser](../../com.groupdocs.parser/parser) για το περιεχόμενο του στοιχείου.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Δημιουργεί το αντικείμενο [Parser](../../com.groupdocs.parser/parser) για το περιεχόμενο του στοιχείου με τις [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του περιεχομένου του αντικειμένου. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Δημιουργεί το αντικείμενο [Parser](../../com.groupdocs.parser/parser) για το περιεχόμενο του στοιχείου με τις [LoadOptions](../../com.groupdocs.parser.options/loadoptions) και τις [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Οι επιλογές για το άνοιγμα του περιεχομένου του αντικειμένου. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Οι ρυθμίσεις του αναλυτή που χρησιμοποιούνται για την προσαρμογή της εξαγωγής δεδομένων. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Ανιχνεύει τον τύπο αρχείου του στοιχείου του κοντέινερ.


detectionMode
Η παράμετρος παρέχει τη δυνατότητα ελέγχου της ανίχνευσης τύπου αρχείου:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Το παρακάτω παράδειγμα δείχνει πώς να ανιχνεύσετε τον τύπο αρχείου του αντικειμένου container:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Ορίζει μια λειτουργία εντοπισμού τύπου αρχείου. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

