---
title: "DocumentPageData"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τα δεδομένα της σελίδας του εγγράφου."
type: docs
weight: 12
url: /el/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Αναπαριστά τα δεδομένα της σελίδας του εγγράφου. Αποτελείται από αντικείμενα [FieldData](../../com.groupdocs.parser.data/fielddata) που περιέχουν δεδομένα πεδίου από τη σελίδα του εγγράφου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Λαμβάνει τον δείκτη της σελίδας. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | πεδία | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | Η συλλογή των δεδομένων πεδίων. |
|
|  | pageIndex | int | Ο δείκτης σελίδας με μηδενική βάση. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Λαμβάνει τον δείκτη της σελίδας.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της σελίδας.

