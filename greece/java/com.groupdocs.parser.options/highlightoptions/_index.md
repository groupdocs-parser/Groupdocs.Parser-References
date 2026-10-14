---
title: "HighlightOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή ενός επισημασμένου μπλοκ κειμένου γύρω από το ευρεθέν κείμενο σε σενάρια αναζήτησης."
type: docs
weight: 22
url: /el/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή ενός επισημάνσματος (ενός μπλοκ κειμένου γύρω από το ευρεθέν κείμενο σε σενάρια αναζήτησης).

Μια παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) χρησιμοποιείται ως παράμετρος στη μέθοδο [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
Δείτε τα παραδείγματα χρήσης εκεί.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) χωρίς ορισμένα όρια. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) που χρησιμοποιείται για την εξαγωγή επισημάνσεως σταθερού μήκους. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) που χρησιμοποιείται για την εξαγωγή επισημάνσεως περιορισμένης σε γραμμή. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) που χρησιμοποιείται για την εξαγωγή επισημάνσεως με σταθερό αριθμό λέξεων. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Λαμβάνει το μέγιστο μήκος κειμένου. |
|
|  | [getWordCount()](#getWordCount--) | Λαμβάνει το μέγιστο πλήθος λέξεων. |
|
|  | [isLineLimited()](#isLineLimited--) | Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή επισημάνσεως περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Ορίζει το μέγιστο μήκος κειμένου. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Ορίζει το μέγιστο πλήθος λέξεων. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Ορίζει την τιμή που υποδεικνύει εάν η εξαγωγή επισημάνσεως περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) χωρίς ορισμένα όρια. Ορίστε τουλάχιστον ένα από τα #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) πριν το περάσετε στον αναλυτή.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) που χρησιμοποιείται για την εξαγωγή επισημάνσεως σταθερού μήκους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | maxLength | int | Το μέγιστο μήκος κειμένου. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) που χρησιμοποιείται για την εξαγωγή επισημάνσεως περιορισμένης σε γραμμή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Το μέγιστο μήκος κειμένου. |
|
|  | isLineLimited | boolean | Η τιμή που υποδεικνύει εάν η εξαγωγή επισήμανσης περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) που χρησιμοποιείται για την εξαγωγή επισημάνσεως με σταθερό αριθμό λέξεων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Το μέγιστο μήκος κειμένου. |
|
|  | wordCount | int | Το μέγιστο πλήθος λέξεων. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Το μέγιστο μήκος κειμένου. |
|
|  | wordCount | java.lang.Integer | Το μέγιστο πλήθος λέξεων. |
|
|  | isLineLimited | boolean | Η τιμή που υποδεικνύει εάν η εξαγωγή επισήμανσης περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Λαμβάνει το μέγιστο μήκος κειμένου.


**Returns:**
java.lang.Integer - Μια θετική ακέραια τιμή που αντιπροσωπεύει το μέγιστο μήκος κειμένου·  null  εάν το μήκος κειμένου δεν περιορίζεται.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Λαμβάνει το μέγιστο πλήθος λέξεων.


**Returns:**
java.lang.Integer - Μια θετική ακέραια τιμή που αντιπροσωπεύει το μέγιστο πλήθος λέξεων·  null  εάν το πλήθος λέξεων δεν περιορίζεται.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Λαμβάνει την τιμή που υποδεικνύει εάν η εξαγωγή επισημάνσεως περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου.


**Returns:**
boolean -  true  εάν η εξαγωγή επισήμανσης περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου· διαφορετικά,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Ορίζει το μέγιστο μήκος κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Ένας μη αρνητικός ακέραιος·  null  για την αφαίρεση του περιορισμού μήκους. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Ορίζει το μέγιστο πλήθος λέξεων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Ένας μη αρνητικός ακέραιος·  null  για την αφαίρεση του περιορισμού πλήθους λέξεων. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Ορίζει την τιμή που υποδεικνύει εάν η εξαγωγή επισημάνσεως περιορίζεται από την αρχή (ή το τέλος) μιας γραμμής κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lineLimited | boolean | true  για περιορισμό με τα όρια της γραμμής. |
|

