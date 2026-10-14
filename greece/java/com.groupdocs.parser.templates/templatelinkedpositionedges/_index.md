---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις άκρες του συνδεδεμένου πεδίου όπου αναζητείται το πεδίο κειμένου."
type: docs
weight: 16
url: /el/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Παρέχει τις άκρες του συνδεδεμένου πεδίου όπου το πεδίο κειμένου αναζητείται. Το [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) χρησιμοποιείται στην κλάση [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Λαμβάνει την τιμή που υποδεικνύει εάν η παρουσία είναι κενή. |
|
|  | [isLeft()](#isLeft--) | Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από αριστερά του συνδεδεμένου πεδίου. |
|
|  | [isTop()](#isTop--) | Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από πάνω του συνδεδεμένου πεδίου. |
|
|  | [isRight()](#isRight--) | Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από δεξιά του συνδεδεμένου πεδίου. |
|
|  | [isBottom()](#isBottom--) | Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από κάτω του συνδεδεμένου πεδίου. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Μετατρέπει την αναπαράσταση συμβολοσειράς των άκρων στην αντίστοιχη κλάση. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | left | boolean | Η τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από αριστερά του συνδεδεμένου πεδίου. |
|
|  | top | boolean | Η τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από πάνω του συνδεδεμένου πεδίου. |
|
|  | δεξιά | boolean | Η τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από τη δεξιά του συνδεδεμένου πεδίου. |
|
|  | κάτω | boolean | Η τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από το κάτω του συνδεδεμένου πεδίου. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η παρουσία είναι κενή.


**Returns:**
boolean -  true  αν η παρουσία είναι κενή (όλα τα πεδία είναι  false ); διαφορετικά,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από αριστερά του συνδεδεμένου πεδίου.


**Returns:**
boolean -  true  αν ένα πεδίο αναζητείται από την αριστερά του συνδεδεμένου πεδίου· διαφορετικά,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από πάνω του συνδεδεμένου πεδίου.


**Returns:**
boolean -  true  αν ένα πεδίο αναζητείται από την κορυφή του συνδεδεμένου πεδίου· διαφορετικά,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από δεξιά του συνδεδεμένου πεδίου.


**Returns:**
boolean -  true  αν ένα πεδίο αναζητείται από τη δεξιά του συνδεδεμένου πεδίου· διαφορετικά,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Λαμβάνει την τιμή που υποδεικνύει εάν ένα πεδίο αναζητείται από κάτω του συνδεδεμένου πεδίου.


**Returns:**
boolean -  true  αν ένα πεδίο αναζητείται από το κάτω του συνδεδεμένου πεδίου· διαφορετικά,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Μετατρέπει την αναπαράσταση συμβολοσειράς των άκρων στην αντίστοιχη κλάση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | s | java.lang.String | Μια συμβολοσειρά που περιέχει άκρα για μετατροπή. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
