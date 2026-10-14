---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή περιοχών πινάκων σελίδας."
type: docs
weight: 31
url: /el/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή περιοχών πινάκων σελίδας.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) με ένα ορθογώνιο αναζήτησης και χωρίς σταθερή διάταξη. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Λαμβάνει τη διάταξη πίνακα που ορίζει τον πίνακα σε μια σελίδα. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Η διάταξη πίνακα που ορίζει τον πίνακα σε μια σελίδα. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) με ένα ορθογώνιο αναζήτησης και χωρίς σταθερή διάταξη.

Χρήσιμο για τον περιορισμό των αυτόματα ανιχνευμένων πινάκων σε μια περιοχή της σελίδας. Αντιστοιχεί στο C#

new PageTableAreaOptions(null) { Rectangle = ... }
πρότυπο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή στη σελίδα όπου πρέπει να εντοπιστούν οι πίνακες· περάστε  null  για να αναζητήσετε ολόκληρη τη σελίδα. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Λαμβάνει τη διάταξη πίνακα που ορίζει τον πίνακα σε μια σελίδα.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

