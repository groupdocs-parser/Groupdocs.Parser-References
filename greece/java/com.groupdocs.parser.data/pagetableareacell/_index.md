---
title: "PageTableAreaCell"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει ένα κελί πίνακα που χρησιμοποιείται στην κλάση."
type: docs
weight: 23
url: /el/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Αντιπροσωπεύει ένα κελί πίνακα που χρησιμοποιείται στην κλάση [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Αρχικοποιεί μια νέα εμφάνιση της κλάσης [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Αρχικοποιεί μια νέα εμφάνιση της κλάσης [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Λαμβάνει τον δείκτη της γραμμής. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Λαμβάνει τον δείκτη της στήλης. |
|
|  | [getRowSpan()](#getRowSpan--) | Λαμβάνει το συνολικό αριθμό γραμμών που περιέχουν το κελί του πίνακα. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Λαμβάνει το συνολικό αριθμό στηλών που περιέχουν το κελί του πίνακα. |
|
|  | [getPageArea()](#getPageArea--) | Λαμβάνει την τιμή του κελιού του πίνακα. |
|
|  | [getText()](#getText--) | Λαμβάνει την κειμενική τιμή του κελιού του πίνακα. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Αρχικοποιεί μια νέα εμφάνιση της κλάσης [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rowIndex | int | Ο δείκτης μηδενικής βάσης της γραμμής. |
|
|  | columnIndex | int | Ο δείκτης μηδενικής βάσης της στήλης. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Η τιμή του κελιού του πίνακα. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Αρχικοποιεί μια νέα εμφάνιση της κλάσης [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rowIndex | int | Ο δείκτης μηδενικής βάσης της γραμμής. |
|
|  | columnIndex | int | Ο δείκτης μηδενικής βάσης της στήλης. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Η τιμή του κελιού του πίνακα. |
|
|  | rowSpan | int | Το συνολικό αριθμό γραμμών που περιέχουν το κελί του πίνακα. |
|
|  | columnSpan | int | Το συνολικό αριθμό στηλών που περιέχουν το κελί του πίνακα. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Λαμβάνει τον δείκτη της γραμμής.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της πρώτης γραμμής που περιέχει το κελί του πίνακα.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Λαμβάνει τον δείκτη της στήλης.


**Returns:**
int - Ένας δείκτης μηδενικής βάσης της πρώτης στήλης που περιέχει το κελί του πίνακα.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Λαμβάνει το συνολικό αριθμό γραμμών που περιέχουν το κελί του πίνακα.


**Returns:**
int - Μια θετική ακέραια τιμή που αντιπροσωπεύει το συνολικό αριθμό γραμμών που περιέχουν το κελί του πίνακα.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Λαμβάνει το συνολικό αριθμό στηλών που περιέχουν το κελί του πίνακα.


**Returns:**
int - Μια θετική ακέραια τιμή που αντιπροσωπεύει το συνολικό αριθμό στηλών που περιέχουν το κελί του πίνακα.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Λαμβάνει την τιμή του κελιού του πίνακα.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει την κειμενική τιμή του κελιού του πίνακα.


**Returns:**
java.lang.String - Συμβολοσειρά που αντιπροσωπεύει μια τιμή κειμένου του κελιού· null εάν το κελί δεν περιέχει τιμή κειμένου.

