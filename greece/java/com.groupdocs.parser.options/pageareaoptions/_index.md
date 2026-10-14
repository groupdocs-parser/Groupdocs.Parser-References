---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή περιοχών σελίδας."
type: docs
weight: 28
url: /el/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή περιοχών σελίδας.

Μια παρουσία της κλάσης [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) χρησιμοποιείται ως παράμετρος στη μέθοδο [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
και στις μεθόδους [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) με το μέγεθος του αγνοημένου περιγράμματος. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Λαμβάνει την ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Λαμβάνει το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) με το μέγεθος του αγνοημένου περιγράμματος.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|
|  | rectangleTolerance | double | Το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετριέται ως κλάσμα του ύψους ενός στοιχείου κειμένου. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Λαμβάνει την ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Λαμβάνει το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετριέται ως κλάσμα του ύψους ενός στοιχείου κειμένου.


**Returns:**
double - Η τιμή double από 0 (χωρίς περίγραμμα) έως 1 (αγνόηση ολόκληρου του στοιχείου).

