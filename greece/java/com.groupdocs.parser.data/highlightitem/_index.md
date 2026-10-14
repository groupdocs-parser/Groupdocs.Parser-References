---
title: "HighlightItem"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια επισήμανση ενός τμήματος του κειμένου που συνήθως χρησιμοποιείται για να εξηγήσει το πλαίσιο του ευρεθέντος κειμένου στη λειτουργία αναζήτησης."
type: docs
weight: 14
url: /el/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Αντιπροσωπεύει μια επισήμανση, ένα τμήμα του κειμένου που συνήθως χρησιμοποιείται για την εξήγηση του πλαισίου του ευρεθέντος κειμένου στη λειτουργία αναζήτησης.

Μια παρουσία της κλάσης [HighlightItem](../../com.groupdocs.parser.data/highlightitem) χρησιμοποιείται ως τιμή επιστροφής της μεθόδου [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) ,
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getPosition()](#getPosition--) | Λαμβάνει τη θέση στο κείμενο του εγγράφου. |
|
|  | [getText()](#getText--) | Λαμβάνει το κείμενο της επισήμανσης. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | θέση | int | Η θέση στο κείμενο του εγγράφου. |
|
|  | κείμενο | java.lang.String | Το κείμενο της επισήμανσης. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Λαμβάνει τη θέση στο κείμενο του εγγράφου.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της αρχικής θέσης της επισήμανσης.

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει το κείμενο της επισήμανσης.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το κείμενο της επισήμανσης.

