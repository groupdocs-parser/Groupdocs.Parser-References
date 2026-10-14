---
title: "DocumentInfo"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τις πληροφορίες του εγγράφου."
type: docs
weight: 11
url: /el/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Αντιπροσωπεύει τις πληροφορίες του εγγράφου.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileType()](#getFileType--) | Λαμβάνει τον τύπο του εγγράφου. |
|
|  | [getPageCount()](#getPageCount--) | Λαμβάνει τον συνολικό αριθμό σελίδων του εγγράφου. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Λαμβάνει τον συνολικό αριθμό ακατέργαστων σελίδων του εγγράφου. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το μέγεθος του εγγράφου σε byte. |
|
|  | [getPages()](#getPages--) | Λαμβάνει τις πληροφορίες σχετικά με τις σελίδες, όπως ο δείκτης και το μέγεθος της σελίδας. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Λαμβάνει τον τύπο του εγγράφου.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Λαμβάνει τον συνολικό αριθμό σελίδων του εγγράφου.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει τον συνολικό αριθμό σελίδων.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Λαμβάνει τον συνολικό αριθμό ακατέργαστων σελίδων του εγγράφου.

Χρησιμοποιήστε την ιδιότητα [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) αντί για την ιδιότητα [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) για εξαγωγή ακατέργαστου κειμένου.
Ορισμένα έγγραφα έχουν διαφορετικούς αριθμούς σελίδων σε ακριβείς και ακατέργαστες λειτουργίες εξαγωγής κειμένου.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει τον συνολικό αριθμό ακατέργαστων σελίδων.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Λαμβάνει το μέγεθος του εγγράφου σε byte.


**Returns:**
long - Μια ακέραια τιμή που αντιπροσωπεύει το μέγεθος του εγγράφου σε byte.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Λαμβάνει τις πληροφορίες σχετικά με τις σελίδες, όπως ο δείκτης και το μέγεθος της σελίδας.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Μια συλλογή με στιγμιότυπα των κλάσεων [PageInfo](../../com.groupdocs.parser.options/pageinfo).

