---
title: "PageRenderInfo"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αναπαριστά τις πληροφορίες για το πώς αποδίδεται μια σελίδα."
type: docs
weight: 30
url: /el/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Αναπαριστά τις πληροφορίες για το πώς αποδίδεται μια σελίδα.

Ορισμένα έγγραφα (υπολογιστικά φύλλα, για παράδειγμα) δεν είναι δυνατόν να αποδοθούν σε μια σελίδα
ως μία ενιαία εικόνα. Για αυτά τα έγγραφα, μια σελίδα αποδίδεται ως σύνολο πλακιδίων.
Αυτά τα πλακίδια τοποθετούνται στον ορθογώνιο πίνακα.


RowCount
και
ColumnCount
αντιπροσωπεύουν τον συνολικό αριθμό γραμμών και στηλών
αυτού του πίνακα. Εάν η σελίδα του εγγράφου αποδοθεί σε μία ενιαία εικόνα, αυτές οι ιδιότητες είναι ίσες με 1.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Αποκτά τον αριθμό της σελίδας. |
|
|  | [getRowCount()](#getRowCount--) | Αποκτά τον συνολικό αριθμό γραμμών πλακιδίων. |
|
|  | [getColumnCount()](#getColumnCount--) | Αποκτά τον συνολικό αριθμό στηλών πλακιδίων. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Επιστρέφει το δείκτη της στήλης όπου το πλακίδιο με  tileIndex  τοποθετείται. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Επιστρέφει το δείκτη της γραμμής όπου το πλακίδιο με  tileIndex  τοποθετείται. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageNumber | int | Ο αριθμός της σελίδας (ξεκινά από 1). |
|
|  | rowCount | int | Συνολικός αριθμός γραμμών πλακιδίων. |
|
|  | columnCount | int | Συνολικός αριθμός στηλών πλακιδίων. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Αποκτά τον αριθμό της σελίδας.


**Returns:**
int - Η ακέραια τιμή που αντιπροσωπεύει τον αριθμό της σελίδας (ξεκινά από 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Αποκτά τον συνολικό αριθμό γραμμών πλακιδίων.


**Returns:**
int - Η ακέραια τιμή που αντιπροσωπεύει τον συνολικό αριθμό γραμμών πλακιδίων.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Αποκτά τον συνολικό αριθμό στηλών πλακιδίων.


**Returns:**
int - Η ακέραια τιμή που αντιπροσωπεύει τον συνολικό αριθμό στηλών πλακιδίων.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Επιστρέφει το δείκτη της στήλης όπου το πλακίδιο με  tileIndex  τοποθετείται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | tileIndex | int | Ο δείκτης του πλακιδίου με βάση το μηδέν. |
|

**Returns:**
int - Η ακέραια τιμή μηδενικής βάσης που αντιπροσωπεύει τον δείκτη στήλης.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Επιστρέφει το δείκτη της γραμμής όπου το πλακίδιο με  tileIndex  τοποθετείται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | tileIndex | int | Ο δείκτης του πλακιδίου με βάση το μηδέν. |
|

**Returns:**
int - Η ακέραια τιμή μηδενικής βάσης που αντιπροσωπεύει τον δείκτη γραμμής.

