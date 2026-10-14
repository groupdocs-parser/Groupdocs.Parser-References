---
title: "TemplateOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την ανάλυση μέσω της λειτουργικότητας προτύπου."
type: docs
weight: 17
url: /el/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την ανάλυση μέσω της λειτουργικότητας προτύπου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Λαμβάνει το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangleTolerance | double | Το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετριέται ως κλάσμα του ύψους ενός στοιχείου κειμένου. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Λαμβάνει το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετριέται ως κλάσμα του ύψους ενός στοιχείου κειμένου.


**Returns:**
double - Η τιμή double από 0 (χωρίς περίγραμμα) έως 1 (αγνόηση ολόκληρου του στοιχείου).

