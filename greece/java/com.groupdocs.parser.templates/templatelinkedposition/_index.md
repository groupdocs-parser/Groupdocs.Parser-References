---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη θέση του πεδίου προτύπου που χρησιμοποιεί το συνδεδεμένο πεδίο."
type: docs
weight: 15
url: /el/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Παρέχει τη θέση του πεδίου προτύπου που χρησιμοποιεί το συνδεδεμένο πεδίο.

Το παρακάτω παράδειγμα δείχνει τον κώδικα για την περίπτωση εάν είναι γνωστό ότι το πεδίο με αριθμό τιμολογίου
τοποθετείται δεξιά της συμβολοσειράς "Invoice number" χρησιμοποιείται ο παρακάτω κώδικας:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) με όνομα UPPER CASE. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Λαμβάνει το όνομα του συνδεδεμένου πεδίου. |
|
|  | [getSearchArea()](#getSearchArea--) | Λαμβάνει το μέγεθος της περιοχής όπου γίνεται η αναζήτηση ενός πεδίου. |
|
|  | [isAutoScale()](#isAutoScale--) | Λαμβάνει την τιμή που υποδεικνύει εάν το  SearchArea  κλιμακώνεται από το μέγεθος του συνδεδεμένου πεδίου. |
|
|  | [getEdges()](#getEdges--) | Λαμβάνει τις άκρες του συνδεδεμένου πεδίου όπου γίνεται η αναζήτηση ενός πεδίου. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Το όνομα του συνδεδεμένου πεδίου. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Το μέγεθος της περιοχής όπου γίνεται η αναζήτηση ενός πεδίου. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Τα άκρα του συνδεδεμένου πεδίου όπου γίνεται η αναζήτηση ενός πεδίου. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) με όνομα UPPER CASE.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Το όνομα του συνδεδεμένου πεδίου. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Το μέγεθος της περιοχής όπου γίνεται η αναζήτηση ενός πεδίου. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Τα άκρα του συνδεδεμένου πεδίου όπου γίνεται η αναζήτηση ενός πεδίου. |
|
|  | autoScale | boolean | Η τιμή που υποδεικνύει εάν η περιοχή αναζήτησης (searchArea) κλιμακώνεται με βάση το μέγεθος του συνδεδεμένου πεδίου. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Το όνομα του συνδεδεμένου πεδίου. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Το μέγεθος της περιοχής όπου γίνεται η αναζήτηση ενός πεδίου. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Τα άκρα του συνδεδεμένου πεδίου όπου γίνεται η αναζήτηση ενός πεδίου. |
|
|  | autoScale | boolean | Η τιμή που υποδεικνύει εάν η περιοχή αναζήτησης (searchArea) κλιμακώνεται με βάση το μέγεθος του συνδεδεμένου πεδίου.\\ |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Λαμβάνει το όνομα του συνδεδεμένου πεδίου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς με κεφαλαία γράμματα που αντιπροσωπεύει το όνομα του συνδεδεμένου πεδίου.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Λαμβάνει το μέγεθος της περιοχής όπου γίνεται η αναζήτηση ενός πεδίου.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Λαμβάνει την τιμή που υποδεικνύει εάν το  SearchArea  κλιμακώνεται από το μέγεθος του συνδεδεμένου πεδίου.


**Returns:**
java.lang.Boolean - {code true} εάν η SearchArea κλιμακώνεται με βάση το μέγεθος του συνδεδεμένου πεδίου· διαφορετικά, false.

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Λαμβάνει τις άκρες του συνδεδεμένου πεδίου όπου γίνεται η αναζήτηση ενός πεδίου.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Δημιουργεί ένα αντίγραφο της τρέχουσας θέσης με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοθέντα παράγοντα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| παράγοντας | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
