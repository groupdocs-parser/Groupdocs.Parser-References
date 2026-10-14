---
title: "FileInfo"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αναπαριστά τις πληροφορίες του αρχείου."
type: docs
weight: 19
url: /el/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

Αναπαριστά τις πληροφορίες του αρχείου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileType()](#getFileType--) | Λαμβάνει τον τύπο του εγγράφου. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το μέγεθος του εγγράφου σε byte. |
|
|  | [isEncrypted()](#isEncrypted--) | Λαμβάνει μια τιμή που αντιπροσωπεύει εάν ένα αρχείο είναι προστατευμένο με κωδικό. |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| encrypted | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Λαμβάνει τον τύπο του εγγράφου.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


Λαμβάνει το μέγεθος του εγγράφου σε byte.


**Returns:**
long - Μια ακέραια τιμή που αντιπροσωπεύει το μέγεθος του εγγράφου σε byte.

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Λαμβάνει μια τιμή που αντιπροσωπεύει εάν ένα αρχείο είναι προστατευμένο με κωδικό.


**Returns:**
boolean - Μια boolean true εάν ένα αρχείο είναι προστατευμένο με κωδικό· διαφορετικά false.

