---
title: "MetadataItem"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει ένα στοιχείο μεταδεδομένων που χρησιμοποιείται σε στοιχεία κοντέινερ και στη λειτουργία εξαγωγής μεταδεδομένων."
type: docs
weight: 15
url: /el/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Αντιπροσωπεύει ένα στοιχείο μεταδεδομένων που χρησιμοποιείται σε στοιχεία κοντέινερ και στη λειτουργία εξαγωγής μεταδεδομένων.

Ένα στιγμιότυπο της κλάσης [MetadataItem](../../com.groupdocs.parser.data/metadataitem) χρησιμοποιείται ως τιμή επιστροφής της μεθόδου [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
και ως στοιχείο στη συλλογή [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getName()](#getName--) | Λαμβάνει το όνομα του στοιχείου μεταδεδομένων. |
|
|  | [getValue()](#getValue--) | Λαμβάνει την τιμή του στοιχείου μεταδεδομένων. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | όνομα | java.lang.String | Το όνομα του στοιχείου μεταδεδομένων. |
|
|  | τιμή | java.lang.String | Η τιμή του στοιχείου μεταδεδομένων. |
|

### getName() {#getName--}
```
public String getName()
```


Λαμβάνει το όνομα του στοιχείου μεταδεδομένων.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το όνομα του στοιχείου μεταδεδομένων.

### getValue() {#getValue--}
```
public String getValue()
```


Λαμβάνει την τιμή του στοιχείου μεταδεδομένων.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει την τιμή του στοιχείου μεταδεδομένων.

