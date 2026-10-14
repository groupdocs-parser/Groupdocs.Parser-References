---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει παραμέτρους για τους αλγόριθμους ανίχνευσης πίνακα."
type: docs
weight: 22
url: /el/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Παρέχει παραμέτρους για τους αλγόριθμους ανίχνευσης πίνακα.

Υπάρχουν δύο αλγόριθμοι για την ανίχνευση ενός πίνακα:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

Σε ορισμένες περιπτώσεις όταν οι αλγόριθμοι δεν μπορούν να εντοπίσουν έναν πίνακα ή το κάνουν με μη ακριβή τρόπο, χρησιμοποιείται η κλάση [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Αποκτά την ορθογώνια περιοχή που περιέχει τον πίνακα. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Αποκτά τους διαχωριστές των στηλών του πίνακα. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Λαμβάνει την τιμή που υποδεικνύει εάν ο πίνακας έχει συγχωνευμένα κελιά. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Λαμβάνει τον ελάχιστο αριθμό των γραμμών του πίνακα. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Λαμβάνει τον ελάχιστο αριθμό των στηλών του πίνακα. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Λαμβάνει το ελάχιστο διάστημα μεταξύ των στηλών του πίνακα. |
|
|  | [scale(double factor)](#scale-double-) | Δημιουργεί ένα αντίγραφο αυτών των παραμέτρων με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοσμένο παράγοντα. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Το ορθογώνιο πεδίο που περιέχει τον πίνακα. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Οι διαχωριστές των στηλών του πίνακα. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Το ορθογώνιο πεδίο που περιέχει τον πίνακα. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Οι διαχωριστές των στηλών του πίνακα. |
|
|  | mergedCells | java.lang.Boolean | Η τιμή που υποδεικνύει εάν ο πίνακας έχει συγχωνευμένα κελιά. |
|
|  | minRowCount | java.lang.Integer | Ο ελάχιστος αριθμός των γραμμών του πίνακα. |
|
|  | minColumnCount | java.lang.Integer | Ο ελάχιστος αριθμός των στηλών του πίνακα. |
|
|  | minVerticalSpace | java.lang.Integer | Ο ελάχιστος χώρος μεταξύ των στηλών του πίνακα. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Αποκτά την ορθογώνια περιοχή που περιέχει τον πίνακα.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Αποκτά τους διαχωριστές των στηλών του πίνακα.


**Returns:**
java.util.List<java.lang.Double> - Μια συλλογή τιμών double που αντιπροσωπεύουν τις x-συντεταγμένες των διαχωριστών των στηλών του πίνακα·  null  αν δεν έχει οριστεί.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Λαμβάνει την τιμή που υποδεικνύει εάν ο πίνακας έχει συγχωνευμένα κελιά.


**Returns:**
java.lang.Boolean -  true  αν ο πίνακας έχει συγχωνευμένα κελιά· διαφορετικά,  false .  null  αν δεν έχει οριστεί.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Λαμβάνει τον ελάχιστο αριθμό των γραμμών του πίνακα.


**Returns:**
java.lang.Integer - Μια ακέραια τιμή που αντιπροσωπεύει τον ελάχιστο αριθμό των γραμμών του πίνακα·  null  αν δεν έχει οριστεί.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Λαμβάνει τον ελάχιστο αριθμό των στηλών του πίνακα.


**Returns:**
java.lang.Integer - Μια ακέραια τιμή που αντιπροσωπεύει τον ελάχιστο αριθμό των στηλών του πίνακα·  null  αν δεν έχει οριστεί.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Λαμβάνει το ελάχιστο διάστημα μεταξύ των στηλών του πίνακα.


**Returns:**
java.lang.Integer - Μια ακέραια τιμή που αντιπροσωπεύει τον ελάχιστο χώρο μεταξύ των στηλών του πίνακα·  null  αν δεν έχει οριστεί.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Δημιουργεί ένα αντίγραφο αυτών των παραμέτρων με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοσμένο παράγοντα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | παράγοντας | double | Ο συντελεστής κλιμάκωσης. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

