---
title: "Size"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει ένα μέγεθος."
type: docs
weight: 28
url: /el/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Αντιπροσωπεύει ένα μέγεθος.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Size](../../com.groupdocs.parser.data/size). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getWidth()](#getWidth--) | Λαμβάνει το πλάτος. |
|
|  | [getHeight()](#getHeight--) | Λαμβάνει το ύψος. |
|
|  | [isEmpty()](#isEmpty--) | Λαμβάνει μια τιμή που υποδεικνύει αν το μέγεθος είναι κενό. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Μετατρέπει την αναπαράσταση συμβολοσειράς ενός μεγέθους στην αντίστοιχη κλάση. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | width | double | Το πλάτος σε εικονοστοιχεία. |
|
|  | height | double | Το ύψος σε εικονοστοιχεία. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Λαμβάνει το πλάτος.


**Returns:**
double - Μια τιμή double που αντιπροσωπεύει το πλάτος σε εικονοστοιχεία.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Λαμβάνει το ύψος.


**Returns:**
double - Μια τιμή double που αντιπροσωπεύει το ύψος σε εικονοστοιχεία.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το μέγεθος είναι κενό.


**Returns:**
boolean -  true  εάν το  πλάτος  και  το ύψος  είναι μηδέν· διαφορετικά,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Μετατρέπει την αναπαράσταση συμβολοσειράς ενός μεγέθους στην αντίστοιχη κλάση. Μια τιμή επιστροφής υποδεικνύει εάν η μετατροπή ολοκληρώθηκε ή απέτυχε.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | s | java.lang.String | Μια συμβολοσειρά που περιέχει ένα μέγεθος για μετατροπή. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
