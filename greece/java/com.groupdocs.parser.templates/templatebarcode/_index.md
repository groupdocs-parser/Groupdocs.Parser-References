---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει το πεδίο barcode του προτύπου."
type: docs
weight: 11
url: /el/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Παρέχει το πεδίο barcode του προτύπου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) με το όνομα σε ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) με το όνομα σε ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Λαμβάνει την ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου barcode. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) με το όνομα σε ΚΕΦΑΛΑΙΑ.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου barcode. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) με το όνομα σε ΚΕΦΑΛΑΙΑ.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου barcode. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου barcode. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου. |
|
|  | όνομα | java.lang.String | Το όνομα του πεδίου barcode. |
|
|  | pageIndex | java.lang.Integer | Μια ακέραια τιμή που αντιπροσωπεύει το δείκτη της σελίδας όπου βρίσκεται το στοιχείο προτύπου· null εάν το στοιχείο προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Λαμβάνει την ορθογώνια περιοχή που περιέχει το πεδίο barcode του προτύπου.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

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
