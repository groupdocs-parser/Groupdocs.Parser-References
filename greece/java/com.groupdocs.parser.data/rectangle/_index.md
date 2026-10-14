---
title: "Ορθογώνιο"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια ορθογώνια περιοχή."
type: docs
weight: 26
url: /el/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Αντιπροσωπεύει μια ορθογώνια περιοχή.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getLeft()](#getLeft--) | Λαμβάνει τη συντεταγμένη x της αριστερής άκρης της ορθογώνιας περιοχής. |
|
|  | [getTop()](#getTop--) | Λαμβάνει τη συντεταγμένη y της επάνω άκρης της ορθογώνιας περιοχής. |
|
|  | [getRight()](#getRight--) | Λαμβάνει τη συντεταγμένη x της δεξιάς άκρης της ορθογώνιας περιοχής. |
|
|  | [getBottom()](#getBottom--) | Λαμβάνει τη συντεταγμένη y του κάτω άκρου της ορθογώνιας περιοχής. |
|
|  | [getPosition()](#getPosition--) | Λαμβάνει τις συντεταγμένες της επάνω αριστερής γωνίας της ορθογώνιας περιοχής. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το μέγεθος. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | left | double | Η συντεταγμένη x της αριστερής άκρης της ορθογώνιας περιοχής. |
|
|  | top | double | Η συντεταγμένη y της επάνω άκρης της ορθογώνιας περιοχής. |
|
|  | δεξιά | double | Η συντεταγμένη x της δεξιάς άκρης της ορθογώνιας περιοχής. |
|
|  | κάτω | double | Η συντεταγμένη y του κάτω άκρου της ορθογώνιας περιοχής. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Οι συντεταγμένες της επάνω αριστερής γωνίας της ορθογώνιας περιοχής. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Το μέγεθος της ορθογώνιας περιοχής. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Λαμβάνει τη συντεταγμένη x της αριστερής άκρης της ορθογώνιας περιοχής.


**Returns:**
double - Διπλή τιμή που αντιπροσωπεύει τη συντεταγμένη x της αριστερής άκρης της ορθογώνιας περιοχής.

### getTop() {#getTop--}
```
public double getTop()
```


Λαμβάνει τη συντεταγμένη y της επάνω άκρης της ορθογώνιας περιοχής.


**Returns:**
double - Διπλή τιμή που αντιπροσωπεύει τη συντεταγμένη y της επάνω άκρης της ορθογώνιας περιοχής.

### getRight() {#getRight--}
```
public double getRight()
```


Λαμβάνει τη συντεταγμένη x της δεξιάς άκρης της ορθογώνιας περιοχής.


**Returns:**
double - Διπλή τιμή που αντιπροσωπεύει τη συντεταγμένη x της δεξιάς άκρης της ορθογώνιας περιοχής.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Λαμβάνει τη συντεταγμένη y του κάτω άκρου της ορθογώνιας περιοχής.


**Returns:**
double - Διπλή τιμή που αντιπροσωπεύει τη συντεταγμένη y του κάτω άκρου της ορθογώνιας περιοχής.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Λαμβάνει τις συντεταγμένες της επάνω αριστερής γωνίας της ορθογώνιας περιοχής.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Λαμβάνει το μέγεθος.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
