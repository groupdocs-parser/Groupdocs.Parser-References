---
title: "TemplateTable"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τον πίνακα προτύπου."
type: docs
weight: 20
url: /el/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Παρέχει τον πίνακα προτύπου.

Υπάρχουν δύο τρόποι για να ορίσετε έναν πίνακα:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable) με όνομα σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable) με όνομα σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable) με όνομα σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getLayout()](#getLayout--) | Λαμβάνει τη διάταξη του πίνακα. |
|
|  | [getParameters()](#getParameters--) | Λαμβάνει τις παραμέτρους για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable) με όνομα σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.

Ο πίνακας προτύπου ορίζεται από τη διάταξη του πίνακα εάν ο πίνακας δεν μπορεί να ανιχνευθεί αυτόματα:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Η διάταξη του πίνακα. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable) με όνομα σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Η διάταξη του πίνακα. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Η διάταξη του πίνακα. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Η διάταξη του πίνακα. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable) με όνομα σε ΑΚΡΟΜΑ ΚΕΦΑΛΑΙΑ.

Εάν ένας πίνακας προτύπου ορίζεται από τις παραμέτρους του ανιχνευτή, ο πίνακας ανιχνεύεται αυτόματα:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Οι παράμετροι για την ανίχνευση του πίνακα σε αυτόματη λειτουργία. |
|
|  | όνομα | java.lang.String | Το όνομα του πίνακα. |
|
|  | pageIndex | java.lang.Integer | Ο δείκτης της σελίδας όπου βρίσκεται ο πίνακας προτύπου·  null  εάν ο πίνακας προτύπου βρίσκεται σε οποιαδήποτε σελίδα. |
|
|  | pageWidth | java.lang.Double | Το πλάτος της σελίδας που χρησιμοποιήθηκε για τη δημιουργία του στοιχείου προτύπου. |
|
|  | useUpperCaseName | boolean | Η τιμή που υποδεικνύει εάν ένα  name  μετατρέπεται σε UPPER CASE. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Λαμβάνει τη διάταξη του πίνακα.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Λαμβάνει τις παραμέτρους για την ανίχνευση του πίνακα σε αυτόματη λειτουργία.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
