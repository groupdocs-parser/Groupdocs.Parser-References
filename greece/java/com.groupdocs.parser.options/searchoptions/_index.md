---
title: "SearchOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την αναζήτηση κειμένου."
type: docs
weight: 35
url: /el/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την αναζήτηση κειμένου.

Μια παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) χρησιμοποιείται ως παράμετρος στη μέθοδο [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Δείτε τα παραδείγματα χρήσης εκεί.

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση με τις επιλογές επισήμανσης για την αριστερή και τη δεξιά εξαγωγή επισήμανσης. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση με τις ίδιες επιλογές επισήμανσης για την αριστερή και τη δεξιά εξαγωγή επισήμανσης. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση χωρίς εξαγωγή επισήμανσης. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση ανά σελίδες και χωρίς εξαγωγή επισήμανσης. |
|
|  | [SearchOptions()](#SearchOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) με προεπιλεγμένες τιμές. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Επιστρέφει την τιμή που υποδεικνύει εάν η περίπτωση κειμένου δεν αγνοείται. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Λαμβάνει την τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Λαμβάνει την τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Λαμβάνει την τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Λαμβάνει τις επιλογές για την αριστερή επισήμανση. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Λαμβάνει τις επιλογές για τη δεξιά επισήμανση. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Λαμβάνει την τιμή που αντιπροσωπεύει το μέγιστο δείκτη της σελίδας προς αναζήτηση. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | matchWholeWord | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | useRegularExpression | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|
|  | searchByPages | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για την αριστερή επισήμανση. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για τη δεξιά επισήμανση. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | matchWholeWord | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | useRegularExpression | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|
|  | maxPageIndex | int | Η τιμή που αντιπροσωπεύει το μέγιστο δείκτη της σελίδας προς αναζήτηση. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για την αριστερή επισήμανση. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για τη δεξιά επισήμανση. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση με τις επιλογές επισήμανσης για την αριστερή και τη δεξιά εξαγωγή επισήμανσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | matchWholeWord | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | useRegularExpression | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για την αριστερή επισήμανση. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για τη δεξιά επισήμανση. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση με τις ίδιες επιλογές επισήμανσης για την αριστερή και τη δεξιά εξαγωγή επισήμανσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | matchWholeWord | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | useRegularExpression | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Οι επιλογές για και τις δύο επισήμανσεις. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση χωρίς εξαγωγή επισήμανσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | matchWholeWord | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | useRegularExpression | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) που χρησιμοποιείται για αναζήτηση ανά σελίδες και χωρίς εξαγωγή επισήμανσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | matchWholeWord | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη. |
|
|  | useRegularExpression | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση. |
|
|  | searchByPages | boolean | Η τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SearchOptions](../../com.groupdocs.parser.options/searchoptions) με προεπιλεγμένες τιμές. Δείτε τις παρατηρήσεις για λεπτομέρειες.

Οι παρακάτω ιδιότητες έχουν προεπιλεγμένες τιμές:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Επιστρέφει την τιμή που υποδεικνύει εάν η περίπτωση κειμένου δεν αγνοείται.


**Returns:**
boolean -  true  εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται· διαφορετικά,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη.


**Returns:**
boolean -  true  εάν η αναζήτηση κειμένου περιορίζεται σε ολόκληρη λέξη· διαφορετικά,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Λαμβάνει την τιμή που υποδεικνύει εάν χρησιμοποιείται κανονική έκφραση.


**Returns:**
boolean -  true  εάν χρησιμοποιείται κανονική έκφραση· διαφορετικά,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η αναζήτηση εκτελείται ανά σελίδες.


**Returns:**
boolean -  true  εάν η αναζήτηση εκτελείται ανά σελίδες· διαφορετικά,  false  και η αναζήτηση εκτελείται σε ολόκληρο το έγγραφο χωρίς να συμπεριλαμβάνεται η τιμή της ιδιότητας [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) στην κλάση [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Λαμβάνει τις επιλογές για την αριστερή επισήμανση.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Λαμβάνει τις επιλογές για τη δεξιά επισήμανση.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Λαμβάνει την τιμή που αντιπροσωπεύει το μέγιστο δείκτη της σελίδας προς αναζήτηση.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει το μέγιστο δείκτη της σελίδας προς αναζήτηση· -1 εάν δεν έχει οριστεί·

