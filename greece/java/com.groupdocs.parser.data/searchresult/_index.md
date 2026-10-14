---
title: "SearchResult"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει το αποτέλεσμα αναζήτησης στη λειτουργία αναζήτησης."
type: docs
weight: 27
url: /el/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Αντιπροσωπεύει το αποτέλεσμα αναζήτησης στη λειτουργία αναζήτησης.

Μια παρουσία της κλάσης SearchResult χρησιμοποιείται ως τιμή επιστροφής της [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-)
και των μεθόδων [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-). Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getPosition()](#getPosition--) | Λαμβάνει τη θέση στο κείμενο του εγγράφου. |
|
|  | [getText()](#getText--) | Λαμβάνει το κείμενο. |
|
|  | [getPageIndex()](#getPageIndex--) | Λαμβάνει τον δείκτη σελίδας όπου βρέθηκε το κείμενο. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Λαμβάνει την αριστερή επισήμανση. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Λαμβάνει τη δεξιά επισήμανση. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | θέση | int | Η θέση στο κείμενο του εγγράφου. |
|
|  | κείμενο | java.lang.String | Το ευρεθέν κείμενο. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης σελίδας όπου βρέθηκε το κείμενο. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Η αριστερή επισήμανση. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Η δεξιά επισήμανση. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | θέση | int | Η θέση στο κείμενο του εγγράφου. |
|
|  | κείμενο | java.lang.String | Το ευρεθέν κείμενο. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης σελίδας όπου βρέθηκε το κείμενο. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Λαμβάνει τη θέση στο κείμενο του εγγράφου.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της αρχικής θέσης του αποτελέσματος αναζήτησης.

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει το κείμενο.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το ευρεθέν κείμενο.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Λαμβάνει τον δείκτη σελίδας όπου βρέθηκε το κείμενο.


**Returns:**
java.lang.Integer - Ένας δείκτης μηδενικής βάσης της σελίδας όπου βρέθηκε το κείμενο·  null  εάν η αναζήτηση πραγματοποιείται σε ολόκληρο το κείμενο του εγγράφου.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Λαμβάνει την αριστερή επισήμανση.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Λαμβάνει τη δεξιά επισήμανση.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

