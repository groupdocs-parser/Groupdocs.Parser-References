---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή περιοχών κειμένου σελίδας."
type: docs
weight: 32
url: /el/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή περιοχών κειμένου σελίδας.

Μία παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) χρησιμοποιείται ως παράμετρος στη μέθοδο [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
και οι μέθοδοι [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) . Δείτε τα παραδείγματα χρήσης εκεί.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με προεπιλεγμένες τιμές. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με την επιλογή χρήσης OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με τη δυνατότητα ορισμού επιλογών OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με την κανονική έκφραση. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με την κανονική έκφραση και το ορθογώνιο πεδίο. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με την κανονική έκφραση, το ορθογώνιο πεδίο και το μέγεθος του αγνοημένου περιγράμματος. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με το μέγεθος του αγνοημένου περιγράμματος. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getExpression()](#getExpression--) | Επιστρέφει την κανονική έκφραση. |
|
|  | [isMatchCase()](#isMatchCase--) | Επιστρέφει την τιμή που υποδεικνύει εάν η περίπτωση κειμένου δεν αγνοείται. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Επιστρέφει την τιμή που υποδεικνύει εάν τα τμήματα είναι ενωμένα. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Επιστρέφει την τιμή που υποδεικνύει εάν η μορφοποίηση κειμένου αγνοείται. |
|
|  | [isUseOcr()](#isUseOcr--) | Αποκτά την τιμή που υποδεικνύει εάν χρησιμοποιείται το OCR Connector για την εξαγωγή κειμένου. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Αποκτά τις πρόσθετες επιλογές για τη λειτουργικότητα OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με προεπιλεγμένες τιμές.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με την επιλογή χρήσης OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | useOcr | boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή κειμένου. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με τη δυνατότητα ορισμού επιλογών OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | useOcr | boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή κειμένου. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Οι πρόσθετες επιλογές για τη λειτουργικότητα OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με την κανονική έκφραση. Οι άλλες επιλογές ορίζονται προεπιλεγμένα (δείτε τις παρατηρήσεις για λεπτομέρειες).

Οι παρακάτω ιδιότητες έχουν προεπιλεγμένες τιμές:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με την κανονική έκφραση και το ορθογώνιο πεδίο. Οι άλλες επιλογές ορίζονται προεπιλεγμένα (δείτε τις παρατηρήσεις για λεπτομέρειες).

Οι παρακάτω ιδιότητες έχουν προεπιλεγμένες τιμές:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με την κανονική έκφραση, το ορθογώνιο πεδίο και το μέγεθος του αγνοημένου περιγράμματος. Οι άλλες επιλογές ορίζονται προεπιλεγμένα (δείτε τις παρατηρήσεις για λεπτομέρειες).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|
|  | rectangleTolerance | double | Το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετριέται ως κλάσμα του ύψους ενός στοιχείου κειμένου. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | uniteSegments | boolean | Η τιμή που υποδεικνύει εάν τα τμήματα είναι ενωμένα. |
|
|  | ignoreFormatting | boolean | Η τιμή που υποδεικνύει εάν η μορφοποίηση του κειμένου αγνοείται. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) με το μέγεθος του αγνοημένου περιγράμματος.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | expression | java.lang.String | Η κανονική έκφραση. |
|
|  | matchCase | boolean | Η τιμή που υποδεικνύει εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται. |
|
|  | uniteSegments | boolean | Η τιμή που υποδεικνύει εάν τα τμήματα είναι ενωμένα. |
|
|  | ignoreFormatting | boolean | Η τιμή που υποδεικνύει εάν η μορφοποίηση του κειμένου αγνοείται. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιέχει τις περιοχές της σελίδας. |
|
|  | rectangleTolerance | double | Το μέγεθος του περιγράμματος που αγνοείται όταν καταγράφεται από την ορθογώνια περιοχή. Μετριέται ως κλάσμα του ύψους ενός στοιχείου κειμένου. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Επιστρέφει την κανονική έκφραση.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει την κανονική έκφραση.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Επιστρέφει την τιμή που υποδεικνύει εάν η περίπτωση κειμένου δεν αγνοείται.


**Returns:**
boolean -  true  εάν η διάκριση πεζών-κεφαλαίων δεν αγνοείται· διαφορετικά,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Επιστρέφει την τιμή που υποδεικνύει εάν τα τμήματα είναι ενωμένα.


**Returns:**
boolean - {code true} εάν τα τμήματα είναι ενωμένα· διαφορετικά, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Επιστρέφει την τιμή που υποδεικνύει εάν η μορφοποίηση κειμένου αγνοείται.


**Returns:**
boolean -  true  εάν η μορφοποίηση του κειμένου αγνοείται· διαφορετικά,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Αποκτά την τιμή που υποδεικνύει εάν χρησιμοποιείται το OCR Connector για την εξαγωγή κειμένου.


**Returns:**
boolean -  true  εάν χρησιμοποιείται η λειτουργία OCR· διαφορετικά,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Αποκτά τις πρόσθετες επιλογές για τη λειτουργικότητα OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

