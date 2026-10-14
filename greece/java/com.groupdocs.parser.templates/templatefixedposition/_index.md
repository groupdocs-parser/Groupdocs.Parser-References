---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη θέση του πεδίου προτύπου που ορίζεται από το ορθογώνιο περιοχή."
type: docs
weight: 13
url: /el/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Παρέχει τη θέση του πεδίου προτύπου που ορίζεται από το ορθογώνιο περιοχή.

Αυτή είναι ο πιο απλός τρόπος για να ορίσετε τη θέση του πεδίου. Απαιτεί τον ορισμό μιας ορθογώνιας περιοχής στη σελίδα που περιορίζει
την τιμή του πεδίου. Όλο το κείμενο που περιέχεται (ακόμη και μερικώς) στην ορθογώνια περιοχή θα εξαχθεί ως τιμή:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Αποκτά την ορθογώνια περιοχή που περιέχει το πεδίο προτύπου. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει το πεδίο προτύπου. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Αποκτά την ορθογώνια περιοχή που περιέχει το πεδίο προτύπου.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

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
