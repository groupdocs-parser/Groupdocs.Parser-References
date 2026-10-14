---
title: "FieldData"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει δεδομένα πεδίου όπως όνομα, δείκτη σελίδας, τιμή πεδίου κ.λπ."
type: docs
weight: 13
url: /el/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Αντιπροσωπεύει δεδομένα πεδίου όπως όνομα, δείκτη σελίδας, τιμή πεδίου κ.λπ. Ανάλογα με το πεδίο, η τιμή μπορεί να είναι κείμενο, εικόνα, πίνακας κ.λπ.

Οι στιγμιότυπα της κλάσης [FieldData](../../com.groupdocs.parser.data/fielddata) χρησιμοποιούνται στη συλλογή [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getName()](#getName--) | Λαμβάνει το όνομα του πεδίου. |
|
|  | [getPageIndex()](#getPageIndex--) | Λαμβάνει τον δείκτη της σελίδας. |
|
|  | [getPageArea()](#getPageArea--) | Λαμβάνει την τιμή του πεδίου. |
|
|  | [getLinkedField()](#getLinkedField--) | Λαμβάνει το συνδεδεμένο πεδίο. |
|
|  | [getText()](#getText--) | Λαμβάνει το κείμενο. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Αποκτά μια τιμή που υποδεικνύει αν ένα  Name  μετατράπηκε σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ. |
|
### getName() {#getName--}
```
public String getName()
```


Λαμβάνει το όνομα του πεδίου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς με κεφαλαία γράμματα που αντιπροσωπεύει το όνομα του πεδίου.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Λαμβάνει τον δείκτη της σελίδας.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της σελίδας που περιέχει το πεδίο.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Λαμβάνει την τιμή του πεδίου.

Ανάλογα με το πεδίο, η ιδιότητα PageArea μπορεί να περιέχει οποιονδήποτε από τους κληρονόμους της κλάσης [PageArea](../../com.groupdocs.parser.data/pagearea).
Για παράδειγμα, η μέθοδος [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) εξάγει μόνο πεδία κειμένου.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Λαμβάνει το συνδεδεμένο πεδίο.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει το κείμενο.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει μια τιμή του κειμένου του πεδίου· null εάν η ιδιότητα [PageArea](../../com.groupdocs.parser.data/pagearea) δεν είναι [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Αποκτά μια τιμή που υποδεικνύει αν ένα  Name  μετατράπηκε σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.


**Returns:**
boolean - Μια λογική τιμή που υποδεικνύει αν ένα  Name  μετατράπηκε σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.

