---
title: "PageTextArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια περιοχή κειμένου σελίδας που χρησιμοποιείται για την αναπαράσταση μιας τιμής κειμένου στη λειτουργία ανάλυσης με πρότυπο ή ανάλυσης φορμών."
type: docs
weight: 24
url: /el/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Αντιπροσωπεύει μια περιοχή κειμένου σελίδας που χρησιμοποιείται για την αναπαράσταση μιας τιμής κειμένου στη λειτουργία ανάλυσης με πρότυπο ή ανάλυσης φορμών.

Μία παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) χρησιμοποιείται ως τιμή επιστροφής των παρακάτω μεθόδων:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Επίσης, μια παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) χρησιμοποιείται ως τιμή της ιδιότητας [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Δείτε τα παραδείγματα χρήσης εκεί.

Η περιοχή κειμένου μπορεί να είναι απλή ή σύνθετη. Στην πρώτη περίπτωση περιέχει κείμενο που περιορίζεται από ένα ορθογώνιο χώρο.
Στη δεύτερη περίπτωση περιέχει άλλες περιοχές κειμένου· οι ιδιότητες κειμένου και πίνακα υπολογίζονται από τις θυγατρικές περιοχές κειμένου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getText()](#getText--) | Λαμβάνει το κείμενο. |
|
|  | [getBaseLine()](#getBaseLine--) | Αποκτά τη γραμμή βάσης. |
|
|  | [getTextStyle()](#getTextStyle--) | Αποκτά το στυλ κειμένου όπως το μέγεθος γραμματοσειράς, το όνομα γραμματοσειράς κλπ. |
|
|  | [getAreas()](#getAreas--) | Αποκτά τη συλλογή των θυγατρικών περιοχών κειμένου σε σελίδες. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | κείμενο | java.lang.String | Η τιμή του κειμένου. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει την περιοχή κειμένου. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει την περιοχή κειμένου. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | κείμενο | java.lang.String | Η τιμή του κειμένου. |
|
|  | baseLine | java.lang.Double | Η γραμμή βάσης του κειμένου. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Το στυλ του κειμένου. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει την περιοχή κειμένου. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει την περιοχή κειμένου. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Η συλλογή των θυγατρικών περιοχών κειμένου σε σελίδες. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει την περιοχή κειμένου. |
|

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει το κείμενο.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει μια τιμή της περιοχής κειμένου σε σελίδα.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Αποκτά τη γραμμή βάσης.


**Returns:**
double - Μια τιμή double που αντιπροσωπεύει τη γραμμή βάσης.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Αποκτά το στυλ κειμένου όπως το μέγεθος γραμματοσειράς, το όνομα γραμματοσειράς κλπ.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Αποκτά τη συλλογή των θυγατρικών περιοχών κειμένου σε σελίδες.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Μια συλλογή των θυγατρικών περιοχών κειμένου σε σελίδες· κενή εάν η περιοχή κειμένου δεν έχει παιδιά.

