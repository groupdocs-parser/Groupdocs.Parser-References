---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη θέση του πεδίου προτύπου που χρησιμοποιεί την κανονική έκφραση."
type: docs
weight: 19
url: /el/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Παρέχει τη θέση του πεδίου προτύπου που χρησιμοποιεί την κανονική έκφραση.

Το παρακάτω παράδειγμα δείχνει την κατάσταση εάν το έγγραφο περιέχει "Invoice Number INV-12345"
τότε το πεδίο προτύπου μπορεί να οριστεί με τον ακόλουθο τρόπο:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

Σε αυτήν την περίπτωση, ως τιμή, εξάγεται ολόκληρη η συμβολοσειρά. Για να εξαχθεί μόνο ένα μέρος της συμβολοσειράς
η ομάδα κανονικής έκφρασης "value" χρησιμοποιείται:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

Σε αυτήν την περίπτωση, ως τιμή, εξάγεται η συμβολοσειρά "INV-3337".

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getExpression()](#getExpression--) | Επιστρέφει την κανονική έκφραση. |
|
|  | [isMatchCase()](#isMatchCase--) | Επιστρέφει την τιμή που υποδεικνύει εάν η περίπτωση κειμένου δεν αγνοείται. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Επιστρέφει την κανονική έκφραση.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει την κανονική έκφραση.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Επιστρέφει την τιμή που υποδεικνύει εάν η περίπτωση κειμένου δεν αγνοείται.


**Returns:**
boolean -  true  εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται· διαφορετικά,  false .

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
