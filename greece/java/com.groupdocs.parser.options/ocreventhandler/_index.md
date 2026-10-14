---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει έναν χειριστή για συμβάντα OCR."
type: docs
weight: 26
url: /el/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Παρέχει έναν χειριστή για συμβάντα OCR.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Λαμβάνει μια λίστα με μηνύματα προειδοποίησης. |
|
|  | [hasWarnings()](#hasWarnings--) | Λαμβάνει την τιμή που υποδεικνύει εάν η λίστα προειδοποιήσεων δεν είναι κενή. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Επιστρέφει μια λίστα προειδοποιητικών μηνυμάτων για τη σελίδα με  pageIndex . |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Ορίζει προειδοποιητικά μηνύματα για τη σελίδα. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Λαμβάνει μια λίστα με μηνύματα προειδοποίησης.


**Returns:**
java.util.List<java.lang.String> - Μια λίστα προειδοποιητικών μηνυμάτων για όλες τις σελίδες.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η λίστα προειδοποιήσεων δεν είναι κενή.


**Returns:**
boolean -  true  εάν η λίστα προειδοποιήσεων δεν είναι κενή· διαφορετικά,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Επιστρέφει μια λίστα προειδοποιητικών μηνυμάτων για τη σελίδα με  pageIndex .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

**Returns:**
java.util.List<java.lang.String> - Μια λίστα προειδοποιητικών μηνυμάτων για τη σελίδα· κενή λίστα εάν δεν υπάρχουν προειδοποιητικά μηνύματα για τη σελίδα.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Ορίζει προειδοποιητικά μηνύματα για τη σελίδα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|
|  | προειδοποιήσεις | java.lang.Iterable<java.lang.String> | Η λίστα προειδοποιητικών μηνυμάτων για τη σελίδα. |
|

