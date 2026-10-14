---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή barcode."
type: docs
weight: 10
url: /el/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή barcode.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions με προεπιλεγμένες τιμές. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions με την ορθογώνια περιοχή. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions με ρυθμίσεις ποιότητας και τύπους κώδικα. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Λαμβάνει την τιμή που υποδεικνύει εάν επιτρέπονται οι λανθασμένοι γραμμωτοί κώδικες. |
|
|  | [getDimension()](#getDimension--) | Λαμβάνει το ελάχιστο μέγεθος του ελάχιστου στοιχείου του γραμμωτού κώδικα. |
|
|  | [getImageQuality()](#getImageQuality--) | Λαμβάνει την ποιότητα μιας εικόνας προέλευσης. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Λαμβάνει την ποιότητα ενός γραμμωτού κώδικα προέλευσης. |
|
|  | [getRectangle()](#getRectangle--) | Λαμβάνει την ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Λαμβάνει τους τύπους των γραμμωτών κωδίκων για ανάγνωση. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Ορίζει την τιμή που υποδεικνύει εάν επιτρέπονται οι λανθασμένοι γραμμωτοί κώδικες. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Ορίζει το ελάχιστο μέγεθος του ελάχιστου στοιχείου του γραμμωτού κώδικα. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Ορίζει την ποιότητα μιας εικόνας προέλευσης. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Ορίζει την ποιότητα ενός γραμμωτού κώδικα προέλευσης. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Ορίζει την ορθογώνια περιοχή που περιέχει γραμμωτούς κώδικες. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Ορίζει τους τύπους των γραμμωτών κωδίκων για ανάγνωση. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions με προεπιλεγμένες τιμές.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions με την ορθογώνια περιοχή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει γραμμωτούς κώδικες. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions με ρυθμίσεις ποιότητας και τύπους κώδικα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Η ποιότητα μιας πηγαίας εικόνας. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Η ποιότητα ενός πηγαίου γραμμωτού κώδικα. |
|
|  | codeTypes | java.lang.String[] | Οι τύποι των γραμμωτών κωδίκων για ανάγνωση. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης BarcodeOptions.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει γραμμωτούς κώδικες. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Η ποιότητα μιας πηγαίας εικόνας. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Η ποιότητα ενός πηγαίου γραμμωτού κώδικα. |
|
|  | dimension | java.lang.Float | Το ελάχιστο μέγεθος του ελάχιστου στοιχείου του γραμμωτού κώδικα. |
|
|  | allowIncorrectBarcodes | boolean | Η τιμή που υποδεικνύει εάν επιτρέπονται οι λανθασμένοι γραμμωτοί κώδικες. |
|
|  | codeTypes | java.lang.String[] | Οι τύποι των γραμμωτών κωδίκων για ανάγνωση. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Λαμβάνει την τιμή που υποδεικνύει εάν επιτρέπονται οι λανθασμένοι γραμμωτοί κώδικες.


**Returns:**
boolean -  true  εάν οι λανθασμένοι γραμμωτοί κώδικες επιτρέπονται· διαφορετικά,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Λαμβάνει το ελάχιστο μέγεθος του ελάχιστου στοιχείου του γραμμωτού κώδικα.


**Returns:**
java.lang.Float - Η τιμή float που αντιπροσωπεύει το ελάχιστο στοιχείο του γραμμωτού κώδικα·  null  εάν χρησιμοποιείται η αυτόματη λειτουργία.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Λαμβάνει την ποιότητα μιας εικόνας προέλευσης.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Λαμβάνει την ποιότητα ενός γραμμωτού κώδικα προέλευσης.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Λαμβάνει την ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Λαμβάνει τους τύπους των γραμμωτών κωδίκων για ανάγνωση.


**Returns:**
java.util.List<java.lang.String> - Η συλλογή μόνο για ανάγνωση που περιέχει τύπους γραμμωτών κωδίκων για ανάγνωση· κενή συλλογή εάν δεν έχει οριστεί.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Ορίζει την τιμή που υποδεικνύει εάν επιτρέπονται οι λανθασμένοι γραμμωτοί κώδικες.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  εάν οι λανθασμένοι γραμμωτοί κώδικες επιτρέπονται. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Ορίζει το ελάχιστο μέγεθος του ελάχιστου στοιχείου του γραμμωτού κώδικα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dimension | java.lang.Float | Το ελάχιστο στοιχείο του γραμμωτού κώδικα·  null  για αυτόματη λειτουργία. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Ορίζει την ποιότητα μιας εικόνας προέλευσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Η λειτουργία ποιότητας εικόνας. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Ορίζει την ποιότητα ενός γραμμωτού κώδικα προέλευσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Η λειτουργία ποιότητας γραμμωτού κώδικα. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Ορίζει την ορθογώνια περιοχή που περιέχει γραμμωτούς κώδικες.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή·  null  για σάρωση ολόκληρης της σελίδας. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Ορίζει τους τύπους των γραμμωτών κωδίκων για ανάγνωση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Οι τύποι των γραμμωτών κωδίκων·  null  ή κενό για όλους τους τύπους. |
|

