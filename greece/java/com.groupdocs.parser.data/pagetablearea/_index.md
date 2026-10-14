---
title: "PageTableArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια περιοχή πίνακα σελίδας που χρησιμοποιείται για την αναπαράσταση πίνακα στη λειτουργία ανάλυσης με πρότυπο."
type: docs
weight: 22
url: /el/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Αντιπροσωπεύει μια περιοχή πίνακα σελίδας που χρησιμοποιείται για την αναπαράσταση πίνακα στη λειτουργία ανάλυσης με πρότυπο.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCells()](#getCells--) | Λαμβάνει τη συλλογή των κελιών. |
|
|  | [getRowCount()](#getRowCount--) | Λαμβάνει τον συνολικό αριθμό των γραμμών του πίνακα. |
|
|  | [getColumnCount()](#getColumnCount--) | Λαμβάνει τον συνολικό αριθμό των στηλών του πίνακα. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Επιστρέφει το ύψος της γραμμής. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Επιστρέφει το πλάτος της στήλης. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Λαμβάνει το κελί του πίνακα με βάση τους δείκτες γραμμής και στήλης. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Σημείωση: το έργο C# σημειώνει αυτόν τον κατασκευαστή ως
εσωτερικό
(commit 954951f). Στην Java, "internal-to-the-assembly"
δεν μεταφράζεται καθαρά σε package-private επειδή οι παραγωγοί (
WordProcessingParser
,
TableAreaParser
,
etc.) ζουν στο
com.groupdocs.parser
, όχι
com.groupdocs.parser.data
. Ο κατασκευαστής επομένως διατηρείται

δημόσιο
οπότε η διασταυρούμενη κατασκευή πακέτων εξακολουθεί να λειτουργεί.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | γραμμές | java.lang.Iterable<java.lang.Double> | Η συλλογή των υψών των γραμμών. |
|
|  | στήλες | java.lang.Iterable<java.lang.Double> | Η συλλογή των πλάτους των στηλών. |
|
|  | κελιά | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | Η συλλογή των κελιών. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει τον πίνακα. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Το ορθογώνιο πεδίο που περιέχει τον πίνακα. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Αποκτά τη συλλογή των κελιών. Μια απλή συλλογή μόνο για ανάγνωση των κελιών του πίνακα.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Μια συλλογή κελιών πίνακα

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Λαμβάνει τον συνολικό αριθμό των γραμμών του πίνακα.


**Returns:**
int - Μια ακέραια τιμή που περιέχει το συνολικό αριθμό των γραμμών του πίνακα.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Λαμβάνει τον συνολικό αριθμό των στηλών του πίνακα.


**Returns:**
int - Μια ακέραια τιμή που περιέχει το συνολικό αριθμό των στηλών του πίνακα.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Επιστρέφει το ύψος της γραμμής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rowIndex | int | Ο δείκτης μηδενικής βάσης της γραμμής. |
|

**Returns:**
double - Μια τιμή double που αντιπροσωπεύει το ύψος της γραμμής.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Επιστρέφει το πλάτος της στήλης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | columnIndex | int | Ο δείκτης μηδενικής βάσης της στήλης. |
|

**Returns:**
double - Μια τιμή double που αντιπροσωπεύει το πλάτος της στήλης.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Λαμβάνει το κελί του πίνακα με βάση τους δείκτες γραμμής και στήλης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rowIndex | int | Ο δείκτης που ξεκινά από το μηδέν της γραμμής του κελιού. |
|
|  | columnIndex | int | Ο δείκτης που ξεκινά από το μηδέν της στήλης του κελιού. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

