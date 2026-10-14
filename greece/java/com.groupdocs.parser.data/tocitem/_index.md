---
title: "TocItem"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει το στοιχείο που χρησιμοποιείται στη λειτουργία εξαγωγής πίνακα περιεχομένων."
type: docs
weight: 31
url: /el/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Αντιπροσωπεύει το στοιχείο που χρησιμοποιείται στη λειτουργία εξαγωγής πίνακα περιεχομένων.

Μία παρουσία της κλάσης [TocItem](../../com.groupdocs.parser.data/tocitem) χρησιμοποιείται ως τιμή επιστροφής της μεθόδου [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) . Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης TocItem. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDepth()](#getDepth--) | Αποκτά το επίπεδο βάθους. |
|
|  | [getText()](#getText--) | Λαμβάνει το κείμενο. |
|
|  | [getPageIndex()](#getPageIndex--) | Λαμβάνει τον δείκτη της σελίδας. |
|
|  | [extractText()](#extractText--) | Εξάγει κείμενο από το έγγραφο στο οποίο αναφέρεται το αντικείμενο TocItem. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης TocItem.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | depth | int | Το επίπεδο βάθους του στοιχείου. |
|
|  | κείμενο | java.lang.String | Το κείμενο του στοιχείου. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας που αναφέρεται από το στοιχείο |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Αποκτά το επίπεδο βάθους.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει το επίπεδο βάθους του στοιχείου.

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει το κείμενο.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το κείμενο του στοιχείου.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Λαμβάνει τον δείκτη της σελίδας.


**Returns:**
java.lang.Integer - Μια ακέραια τιμή που αντιπροσωπεύει τον δείκτη της σελίδας που αναφέρεται από το στοιχείο·  null  εάν δεν έχει οριστεί.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Εξάγει κείμενο από το έγγραφο στο οποίο αναφέρεται το αντικείμενο TocItem.

Το παρακάτω παράδειγμα δείχνει πώς να εξάγετε κείμενο από ένα στοιχείο του πίνακα περιεχομένων:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

