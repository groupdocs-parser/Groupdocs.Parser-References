---
title: "TemplateItem"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει μια βασική αφηρημένη κλάση για στοιχεία προτύπου."
type: docs
weight: 14
url: /el/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Παρέχει μια βασική αφηρημένη κλάση για στοιχεία προτύπου.

Οι κληρονόμοι της κλάσης [TemplateItem](../../com.groupdocs.parser.templates/templateitem) χρησιμοποιούνται στη συλλογή [Template](../../com.groupdocs.parser.templates/template).

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Δημιουργεί ένα αντίγραφο του τρέχοντος στοιχείου με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοσμένο παράγοντα. |
|
|  | [getName()](#getName--) | Αποκτά το όνομα του στοιχείου προτύπου. |
|
|  | [getPageIndex()](#getPageIndex--) | Αποκτά τον δείκτη σελίδας του στοιχείου προτύπου. |
|
|  | [getPageWidth()](#getPageWidth--) | Αποκτά το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Αποκτά μια τιμή που υποδεικνύει αν ένα  Name  μετατράπηκε σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Δημιουργεί ένα αντίγραφο του τρέχοντος στοιχείου με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοσμένο παράγοντα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | παράγοντας | double | Ο συντελεστής κλιμάκωσης. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Αποκτά το όνομα του στοιχείου προτύπου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς με κεφαλαία γράμματα που αντιπροσωπεύει ένα όνομα του στοιχείου προτύπου.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Αποκτά τον δείκτη σελίδας του στοιχείου προτύπου.


**Returns:**
java.lang.Integer - Μια ακέραια τιμή που αντιπροσωπεύει τον δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου·  null  αν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Αποκτά το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου.


**Returns:**
java.lang.Double - Το πλάτος της σελίδας σε εικονοστοιχεία·  null  αν το πλάτος της σελίδας είναι άγνωστο.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Αποκτά μια τιμή που υποδεικνύει αν ένα  Name  μετατράπηκε σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.


**Returns:**
boolean - Μια λογική τιμή που υποδεικνύει αν ένα  Name  μετατράπηκε σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.

