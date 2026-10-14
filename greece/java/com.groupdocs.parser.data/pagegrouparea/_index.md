---
title: "PageGroupArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια ομάδα περιοχών σελίδας που χρησιμοποιείται για την ομαδοποίηση διαφορετικών τύπων μπλοκ της σελίδας του εγγράφου στη λειτουργία ανάλυσης με πρότυπο."
type: docs
weight: 19
url: /el/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Αντιπροσωπεύει μια ομάδα περιοχών σελίδας που χρησιμοποιείται για την ομαδοποίηση διαφορετικών τύπων μπλοκ της σελίδας του εγγράφου στη λειτουργία ανάλυσης με πρότυπο.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getAreas()](#getAreas--) | Λαμβάνει τη συλλογή των ομαδοποιημένων περιοχών σελίδας. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | Η συλλογή των περιοχών σελίδας που θα ομαδοποιηθούν. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει την περιοχή. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Λαμβάνει τη συλλογή των ομαδοποιημένων περιοχών σελίδας.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Μια συλλογή από αντικείμενα [PageArea](../../com.groupdocs.parser.data/pagearea).

