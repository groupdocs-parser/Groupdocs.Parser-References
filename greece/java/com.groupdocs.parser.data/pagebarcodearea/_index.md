---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια περιοχή barcode στη σελίδα που χρησιμοποιείται για την αναπαράσταση της τιμής barcode στη λειτουργία ανάλυσης με πρότυπο."
type: docs
weight: 18
url: /el/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Αντιπροσωπεύει μια περιοχή barcode στη σελίδα που χρησιμοποιείται για την αναπαράσταση της τιμής barcode στη λειτουργία ανάλυσης με πρότυπο.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getValue()](#getValue--) | Επιστρέφει την τιμή του barcode. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Επιστρέφει το όνομα του τύπου barcode. |
|
|  | [getConfidence()](#getConfidence--) | Επιστρέφει το επίπεδο εμπιστοσύνης του αναλυμένου barcode. |
|
|  | [getAngle()](#getAngle--) | Επιστρέφει τη γωνία του barcode. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Η τιμή του barcode. |
|
|  | codeTypeName | java.lang.String | Το όνομα τύπου του barcode. |
|
|  | confidence | int | Το επίπεδο εμπιστοσύνης του επεξεργασμένου barcode. |
|
|  | angle | double | Η γωνία του barcode. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει την περιοχή barcode. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει την περιοχή barcode. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Επιστρέφει την τιμή του barcode.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει μια τιμή της περιοχής barcode της σελίδας.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Επιστρέφει το όνομα του τύπου barcode.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει ένα όνομα τύπου του barcode.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Επιστρέφει το επίπεδο εμπιστοσύνης του αναλυμένου barcode.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει την εμπιστοσύνη του αναλυμένου barcode (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Επιστρέφει τη γωνία του barcode.


**Returns:**
double - Μια ακέραια τιμή που αντιπροσωπεύει τη γωνία του barcode (0-360).

