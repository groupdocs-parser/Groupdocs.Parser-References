---
title: "Point"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει ένα σημείο."
type: docs
weight: 25
url: /el/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Αντιπροσωπεύει ένα σημείο.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Point](../../com.groupdocs.parser.data/point). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getX()](#getX--) | Λαμβάνει την x-συντεταγμένη. |
|
|  | [getY()](#getY--) | Λαμβάνει την y-συντεταγμένη. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Μετατρέπει την αναπαράσταση συμβολοσειράς ενός σημείου στην αντίστοιχη κλάση του. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | x | double | Η x-συντεταγμένη. |
|
|  | y | double | Η y-συντεταγμένη. |
|

### getX() {#getX--}
```
public double getX()
```


Λαμβάνει την x-συντεταγμένη.


**Returns:**
double - Μια τιμή double που αντιπροσωπεύει την x-συντεταγμένη.

### getY() {#getY--}
```
public double getY()
```


Λαμβάνει την y-συντεταγμένη.


**Returns:**
double - Μια τιμή double που αντιπροσωπεύει την y-συντεταγμένη.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Μετατρέπει την αναπαράσταση συμβολοσειράς ενός σημείου στην αντίστοιχη κλάση του. Μια τιμή επιστροφής υποδεικνύει εάν η μετατροπή ολοκληρώθηκε επιτυχώς ή απέτυχε.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | s | java.lang.String | Μια συμβολοσειρά που περιέχει ένα σημείο προς μετατροπή. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
