---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη διάταξη του πίνακα προτύπου που χρησιμοποιείται από την κλάση για τον ορισμό της θέσης του πίνακα."
type: docs
weight: 21
url: /el/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Παρέχει τη διάταξη του πίνακα προτύπου που χρησιμοποιείται από την κλάση [TemplateTable](../../com.groupdocs.parser.templates/templatetable) για τον ορισμό της θέσης του πίνακα.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Αποκτά την ορθογώνια περιοχή που περιέχει τον πίνακα. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Αποκτά τους διαχωριστές των στηλών του πίνακα. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Αποκτά τους διαχωριστές των γραμμών του πίνακα. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Δημιουργεί μια νέα διάταξη με το ίδιο μέγεθος, διαχωριστές και θέση στο σημείο. |
|
|  | [scale(double factor)](#scale-double-) | Δημιουργεί ένα αντίγραφο αυτής της διάταξης με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοθέντα παράγοντα. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Οι διαχωριστές των στηλών του πίνακα. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Οι διαχωριστές των γραμμών του πίνακα. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Αποκτά την ορθογώνια περιοχή που περιέχει τον πίνακα.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Αποκτά τους διαχωριστές των στηλών του πίνακα.


**Returns:**
java.util.List<java.lang.Double> - Μια συλλογή από τιμές double που αντιπροσωπεύουν τις x-συντεταγμένες των διαχωριστών των στηλών του πίνακα.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Αποκτά τους διαχωριστές των γραμμών του πίνακα.


**Returns:**
java.util.List<java.lang.Double> - Μια συλλογή από τιμές double που αντιπροσωπεύουν τις y-συντεταγμένες των διαχωριστών των γραμμών του πίνακα.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Δημιουργεί μια νέα διάταξη με το ίδιο μέγεθος, διαχωριστές και θέση στο σημείο.

Αυτή η λειτουργία επιτρέπει τη μετακίνηση του Table Layout.

Για παράδειγμα, ένα έγγραφο έχει πίνακες σε κάθε σελίδα (ή ένα σύνολο εγγράφων με έναν πίνακα στη σελίδα).
Αυτοί οι πίνακες διαφέρουν ως προς τη θέση και το περιεχόμενο, αλλά έχουν τις ίδιες στήλες και γραμμές. Σε αυτήν την περίπτωση ένας χρήστης
μπορεί να ορίσει το αντικείμενο [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) στο (0, 0) μία φορά και στη συνέχεια να το μετακινήσει στη θέση του συγκεκριμένου πίνακα.

Εάν η θέση του πίνακα εξαρτάται από άλλο αντικείμενο της σελίδας, ένας χρήστης μπορεί να ορίσει το αντικείμενο [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)
βάσει του εγγράφου προτύπου και στη συνέχεια να το μετακινήσει σύμφωνα με ένα αντικείμενο άγκυρας. Για παράδειγμα, εάν αυτός είναι ένας πίνακας περίληψης
και ακολουθείται από πίνακα λεπτομερειών (ο οποίος μπορεί να περιέχει διαφορετικό αριθμό γραμμών). Σε αυτήν την περίπτωση ένας χρήστης μπορεί να ορίσει
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
η μέθοδος επιστρέφει ένα αντίγραφο του τρέχοντος αντικειμένου. Ένας χρήστης μπορεί να περάσει οποιεσδήποτε συντεταγμένες
(ακόμη και αρνητικές - τότε η διάταξη θα μετακινηθεί προς τα αριστερά/πάνω).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | Η θέση της νέας διάταξης. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Δημιουργεί ένα αντίγραφο αυτής της διάταξης με όλες τις συντεταγμένες κλιμακωμένες κατά τον δοθέντα παράγοντα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | παράγοντας | double | Ο συντελεστής κλιμάκωσης. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

