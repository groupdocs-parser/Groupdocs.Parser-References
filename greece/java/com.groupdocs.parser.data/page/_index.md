---
title: "Page"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τις πληροφορίες της σελίδας του εγγράφου όπως δείκτης σελίδας και μέγεθος σελίδας."
type: docs
weight: 16
url: /el/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Αναπαριστά τις πληροφορίες σελίδας του εγγράφου, όπως ο δείκτης σελίδας και το μέγεθος σελίδας. Χρησιμοποιείται για την αναπαράσταση της σελίδας που περιέχει κληρονόμους της κλάσης [PageArea](../../com.groupdocs.parser.data/pagearea) στη λειτουργία ανάλυσης με πρότυπο.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Page](../../com.groupdocs.parser.data/page). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getIndex()](#getIndex--) | Λαμβάνει τον δείκτη της σελίδας. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το μέγεθος της σελίδας. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δείκτης | int | Ο δείκτης σελίδας. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Το μέγεθος σελίδας. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Λαμβάνει τον δείκτη της σελίδας.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της σελίδας.

### getSize() {#getSize--}
```
public Size getSize()
```


Λαμβάνει το μέγεθος της σελίδας.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

