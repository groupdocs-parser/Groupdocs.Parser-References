---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια περιοχή σελίδας που χρησιμοποιείται για την αναπαράσταση ενός υπερσυνδέσμου στη σελίδα."
type: docs
weight: 20
url: /el/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Αντιπροσωπεύει μια περιοχή σελίδας που χρησιμοποιείται για την αναπαράσταση ενός υπερσυνδέσμου στη σελίδα.

Μια παρουσία της κλάσης [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) χρησιμοποιείται ως τιμή επιστροφής των παρακάτω μεθόδων:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Δείτε τα παραδείγματα χρήσης εκεί.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getText()](#getText--) | Λαμβάνει το κείμενο του υπερσυνδέσμου. |
|
|  | [getUrl()](#getUrl--) | Λαμβάνει το URL του υπερσυνδέσμου. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | κείμενο | java.lang.String | Το κείμενο του υπερσυνδέσμου. |
|
|  | url | java.lang.String | Το URL του υπερσυνδέσμου. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Η σελίδα που περιέχει τον υπερσύνδεσμο. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τον υπερσύνδεσμο. |
|

### getText() {#getText--}
```
public String getText()
```


Λαμβάνει το κείμενο του υπερσυνδέσμου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το κείμενο του υπερσυνδέσμου.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Λαμβάνει το URL του υπερσυνδέσμου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το URL του υπερσυνδέσμου.

