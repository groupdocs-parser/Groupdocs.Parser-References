---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη λειτουργικότητα OCR."
type: docs
weight: 25
url: /el/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Παρέχει τη λειτουργικότητα OCR.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή κειμένου υποστηρίζεται. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Αναγνωρίζει κείμενο από  imageStream  ροή. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Αναγνωρίζει περιοχές κειμένου από  imageStream  ροή. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή κειμένου υποστηρίζεται· διαφορετικά,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται· διαφορετικά,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Αναγνωρίζει κείμενο από  imageStream  ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Η αναπαράσταση εικόνας της σελίδας του εγγράφου. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Οι επιλογές OCR. |
|

**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει αναγνωρισμένο κείμενο·  null  εάν η αναγνώριση κειμένου δεν υποστηρίζεται.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Αναγνωρίζει περιοχές κειμένου από  imageStream  ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Η αναπαράσταση εικόνας της σελίδας του εγγράφου. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | Το μέγεθος της σελίδας του εγγράφου. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Οι επιλογές OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Μια συλλογή αντικειμένων [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)·  null  εάν η αναγνώριση περιοχών κειμένου δεν υποστηρίζεται.

