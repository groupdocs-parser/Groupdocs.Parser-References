---
title: "Δυνατότητες"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αναπαριστά τη λίστα υποστηριζόμενων λειτουργιών."
type: docs
weight: 18
url: /el/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Αντιπροσωπεύει τη λίστα των υποστηριζόμενων δυνατοτήτων. Επιτρέπει την απόκτηση πληροφοριών σχετικά με το ποιες δυνατότητες υποστηρίζονται ή όχι για το έγγραφο.

Μια παρουσία αυτής της κλάσης χρησιμοποιείται ως ιδιότητα [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). Δείτε τα παραδείγματα χρήσης εκεί.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Features()](#Features--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Επιστρέφει την τιμή που υποδεικνύει εάν η δυνατότητα υποστηρίζεται. |
|
|  | [isText()](#isText--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή κειμένου υποστηρίζεται. |
|
|  | [isTextPage()](#isTextPage--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή κειμένου σελίδας υποστηρίζεται. |
|
|  | [isFormattedText()](#isFormattedText--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή μορφοποιημένου κειμένου υποστηρίζεται. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή μορφοποιημένου κειμένου σελίδας υποστηρίζεται. |
|
|  | [isSearch()](#isSearch--) | Αποκτά την τιμή που υποδεικνύει εάν η αναζήτηση κειμένου υποστηρίζεται. |
|
|  | [isHighlight()](#isHighlight--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή επισήμανσης υποστηρίζεται. |
|
|  | [isBarcodes()](#isBarcodes--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή γραμμωτών κωδίκων υποστηρίζεται. |
|
|  | [isToc()](#isToc--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή πίνακα περιεχομένων υποστηρίζεται. |
|
|  | [isMetadata()](#isMetadata--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή μεταδεδομένων υποστηρίζεται. |
|
|  | [isContainer()](#isContainer--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή δοχείου υποστηρίζεται. |
|
|  | [isTextAreas()](#isTextAreas--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται. |
|
|  | [isStructure()](#isStructure--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή δομής κειμένου υποστηρίζεται. |
|
|  | [isImages()](#isImages--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή εικόνων υποστηρίζεται. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή υπερσυνδέσμων υποστηρίζεται. |
|
|  | [isTables()](#isTables--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή πινάκων υποστηρίζεται. |
|
|  | [isAnnotations()](#isAnnotations--) | Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή σχολιασμών υποστηρίζεται. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Αποκτά την τιμή που υποδεικνύει εάν η ανάλυση με πρότυπο υποστηρίζεται. |
|
|  | [isParseForm()](#isParseForm--) | Λαμβάνει την τιμή που υποδεικνύει εάν η ανάλυση φόρμας υποστηρίζεται. |
|
|  | [isPreview()](#isPreview--) | Λαμβάνει την τιμή που υποδεικνύει εάν η δημιουργία προεπισκόπησης υποστηρίζεται. |
|
|  | [isPagePreview()](#isPagePreview--) | Λαμβάνει την τιμή που υποδεικνύει εάν η δημιουργία προεπισκόπησης σελίδας υποστηρίζεται. |
|
|  | [isOcr()](#isOcr--) | Λαμβάνει την τιμή που υποδεικνύει εάν η λειτουργία OCR υποστηρίζεται. |
|
|  | [isWorksheet()](#isWorksheet--) | Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή φύλλου εργασίας υποστηρίζεται. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Επιστρέφει την τιμή που υποδεικνύει εάν η δυνατότητα υποστηρίζεται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | featureName | java.lang.String | Το όνομα της δυνατότητας. |
|

**Returns:**
boolean -  true  εάν η δυνατότητα υποστηρίζεται· διαφορετικά,  false .

### isText() {#isText--}
```
public boolean isText()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή κειμένου υποστηρίζεται· διαφορετικά,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή κειμένου σελίδας υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή σελίδας κειμένου υποστηρίζεται· διαφορετικά,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή μορφοποιημένου κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή μορφοποιημένου κειμένου υποστηρίζεται· διαφορετικά,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή μορφοποιημένου κειμένου σελίδας υποστηρίζεται.


**Returns:**
boolean -  true  εάν η μορφοποιημένη σελίδα κειμένου υποστηρίζεται· διαφορετικά,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Αποκτά την τιμή που υποδεικνύει εάν η αναζήτηση κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η αναζήτηση κειμένου υποστηρίζεται· διαφορετικά,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή επισήμανσης υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή επισήμανσης υποστηρίζεται· διαφορετικά,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή γραμμωτών κωδίκων υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή γραμμωτών κωδίκων υποστηρίζεται· διαφορετικά,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή πίνακα περιεχομένων υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή πίνακα περιεχομένων υποστηρίζεται· διαφορετικά,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή μεταδεδομένων υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή μεταδεδομένων υποστηρίζεται· διαφορετικά,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή δοχείου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή υποδοχέα υποστηρίζεται· διαφορετικά,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή περιοχών κειμένου υποστηρίζεται· διαφορετικά,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή δομής κειμένου υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή δομής κειμένου υποστηρίζεται· διαφορετικά,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή εικόνων υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή εικόνων υποστηρίζεται· διαφορετικά,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή υπερσυνδέσμων υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή υπερσυνδέσμων υποστηρίζεται· διαφορετικά,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή πινάκων υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή πινάκων υποστηρίζεται· διαφορετικά,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Αποκτά την τιμή που υποδεικνύει εάν η εξαγωγή σχολιασμών υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή σχολιασμών υποστηρίζεται· διαφορετικά,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Αποκτά την τιμή που υποδεικνύει εάν η ανάλυση με πρότυπο υποστηρίζεται.


**Returns:**
boolean -  true  εάν η ανάλυση με πρότυπο υποστηρίζεται· διαφορετικά,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η ανάλυση φόρμας υποστηρίζεται.


**Returns:**
boolean -  true  εάν η ανάλυση φόρμας υποστηρίζεται· διαφορετικά,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η δημιουργία προεπισκόπησης υποστηρίζεται.


**Returns:**
boolean -  true  εάν η δημιουργία προεπισκόπησης υποστηρίζεται· διαφορετικά,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η δημιουργία προεπισκόπησης σελίδας υποστηρίζεται.


**Returns:**
boolean -  true  εάν η δημιουργία προεπισκόπησης σελίδας υποστηρίζεται· διαφορετικά,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η λειτουργία OCR υποστηρίζεται.


**Returns:**
boolean -  true  εάν η λειτουργικότητα OCR υποστηρίζεται· διαφορετικά,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή φύλλου εργασίας υποστηρίζεται.


**Returns:**
boolean -  true  εάν η εξαγωγή φύλλου εργασίας υποστηρίζεται· διαφορετικά,  false .

