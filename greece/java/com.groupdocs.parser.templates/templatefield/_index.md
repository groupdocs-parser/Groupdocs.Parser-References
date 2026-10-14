---
title: "TemplateField"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει το πεδίο κειμένου του προτύπου."
type: docs
weight: 12
url: /el/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Παρέχει το πεδίο κειμένου του προτύπου.

Τα πεδία κειμένου ορίζονται με βάση τη θέση τους στη σελίδα. Υπάρχουν τρεις τρόποι για να ορίσετε ένα πεδίο κειμένου:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield) με όνομα σε ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield) με όνομα σε ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getPosition()](#getPosition--) | Αποκτά την τιμή που περιγράφει πώς να βρεθεί το πεδίο προτύπου στη σελίδα του εγγράφου. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Η θέση του πεδίου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield) με όνομα σε ΚΕΦΑΛΑΙΑ.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Η θέση του πεδίου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield) με όνομα σε ΚΕΦΑΛΑΙΑ.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Η θέση του πεδίου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Η θέση του πεδίου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Η θέση του πεδίου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Αποκτά την τιμή που περιγράφει πώς να βρεθεί το πεδίο προτύπου στη σελίδα του εγγράφου.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Δημιουργεί ένα αντίγραφο του τρέχοντος στοιχείου με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοσμένο παράγοντα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| παράγοντας | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
