---
title: "LoadOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για το άνοιγμα ενός αρχείου."
type: docs
weight: 24
url: /el/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για το άνοιγμα ενός αρχείου.

Μία παρουσία αυτής της κλάσης χρησιμοποιείται ως παράμετρος στους κατασκευαστές της κλάσης [Parser](../../com.groupdocs.parser/parser):

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Δείτε τα παραδείγματα χρήσης εκεί.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με χρονικό όριο. |
|
|  | [LoadOptions()](#LoadOptions--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κενό Password, FileFormat ίσο με FileFormat.Unknown και προεπιλεγμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με FileFormat ίσο με FileFormat.Unknown και προεπιλεγμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κενό Password και προεπιλεγμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με προεπιλεγμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με προσαρμοσμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Αρχικοποιεί ένα νέο αντικείμενο της πλήρως προσαρμοσμένης κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κενό Password και προεπιλεγμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κωδικό πρόσβασης και προεπιλεγμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με προσαρμοσμένες κωδικοποιήσεις. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Αρχικοποιεί ένα νέο αντικείμενο της πλήρως προσαρμοσμένης κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Λαμβάνει τη μορφή του αρχείου. |
|
|  | [getFileType()](#getFileType--) | Λαμβάνει τον τύπο του αρχείου. |
|
|  | [getPassword()](#getPassword--) | Λαμβάνει τον κωδικό πρόσβασης. |
|
|  | [getCharset()](#getCharset--) | Λαμβάνει την κωδικοποίηση του εγγράφου. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Λαμβάνει την προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
|
|  | [getTimeout()](#getTimeout--) | Λαμβάνει την τιμή που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με χρονικό όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χρονικό όριο | java.time.Duration | Η Duration που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κενό Password, FileFormat ίσο με FileFormat.Unknown και προεπιλεγμένες κωδικοποιήσεις.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με FileFormat ίσο με FileFormat.Unknown και προεπιλεγμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κενό Password και προεπιλεγμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Η μορφή του αρχείου. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με προεπιλεγμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Η μορφή του αρχείου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με προσαρμοσμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Η μορφή του αρχείου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|
|  | charset | java.nio.charset.Charset | Η κωδικοποίηση του εγγράφου. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Αρχικοποιεί ένα νέο αντικείμενο της πλήρως προσαρμοσμένης κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | Η μορφή του αρχείου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|
|  | charset | java.nio.charset.Charset | Η κωδικοποίηση του εγγράφου. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
|
|  | χρονικό όριο | java.time.Duration | Η Duration που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κενό Password και προεπιλεγμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Ο τύπος του αρχείου. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με κωδικό πρόσβασης και προεπιλεγμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Ο τύπος του αρχείου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions) με προσαρμοσμένες κωδικοποιήσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Ο τύπος του αρχείου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|
|  | charset | java.nio.charset.Charset | Η κωδικοποίηση του εγγράφου. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Αρχικοποιεί ένα νέο αντικείμενο της πλήρως προσαρμοσμένης κλάσης [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | Ο τύπος του αρχείου. |
|
|  | κωδικός | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό. |
|
|  | charset | java.nio.charset.Charset | Η κωδικοποίηση του εγγράφου. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | Η προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης. |
|
|  | χρονικό όριο | java.time.Duration | Η Duration που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Λαμβάνει τη μορφή του αρχείου.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Λαμβάνει τον τύπο του αρχείου.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Λαμβάνει τον κωδικό πρόσβασης.


**Returns:**
java.lang.String - Μια τιμή τύπου string που αντιπροσωπεύει έναν κωδικό πρόσβασης για το άνοιγμα του αρχείου που προστατεύεται με κωδικό.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Λαμβάνει την κωδικοποίηση του εγγράφου.


**Returns:**
java.nio.charset.Charset - Μια παρουσία της κλάσης  Charset  που αντιπροσωπεύει την κωδικοποίηση του εγγράφου;  null  εάν δεν έχει οριστεί.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Λαμβάνει την προεπιλεγμένη κωδικοποίηση ANSI που χρησιμοποιείται για την ανίχνευση κωδικοποίησης.


**Returns:**
java.nio.charset.Charset - Μια παρουσία της κλάσης  Charset  που αντιπροσωπεύει την κωδικοποίηση του εγγράφου;  null  εάν δεν έχει οριστεί.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Λαμβάνει την τιμή που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει.


**Returns:**
java.time.Duration - Μια παρουσία της Duration που αντιπροσωπεύει τον αριθμό των χιλιοστών του δευτερολέπτου που πρέπει να περιμένει.

