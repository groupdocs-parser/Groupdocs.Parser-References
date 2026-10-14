---
title: "OcrOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για το OCR Connector."
type: docs
weight: 27
url: /el/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για το OCR Connector.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με προεπιλεγμένες τιμές. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με ορθογώνια περιοχή. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με επιλογές προεπισκόπησης σελίδας. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με αντικείμενο [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με ορθογώνια περιοχή και αντικείμενο [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Λαμβάνει την ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου. |
|
|  | [getHandler()](#getHandler--) | Λαμβάνει τον διαχειριστή συμβάντων για τη σύλληψη γεγονότων OCR. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Λαμβάνει την τιμή που υποδεικνύει εάν χρησιμοποιείται ο ορθογραφικός ελεγκτής. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Λαμβάνει τις επιλογές προεπισκόπησης σελίδας που χρησιμοποιούνται για την απόδοση της σελίδας που παρέχεται στη μηχανή OCR. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Ορίζει τις επιλογές προεπισκόπησης σελίδας που χρησιμοποιούνται για την απόδοση της σελίδας που παρέχεται στη μηχανή OCR. |
|
|  | [getLanguage()](#getLanguage--) | Λαμβάνει τη γλώσσα που χρησιμοποιείται για την οπτική αναγνώριση χαρακτήρων. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Ορίζει τη γλώσσα που χρησιμοποιείται για την οπτική αναγνώριση χαρακτήρων. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Ορίζει την ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Ορίζει τον διαχειριστή συμβάντων για τη σύλληψη συμβάντων OCR. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Ορίζει την τιμή που υποδεικνύει εάν χρησιμοποιείται ο ορθογραφικός ελεγκτής. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με προεπιλεγμένες τιμές.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με ορθογώνια περιοχή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με επιλογές προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Οι επιλογές που χρησιμοποιούνται για την απόδοση της προεπισκόπησης σελίδας που παρέχεται στη μηχανή OCR. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με αντικείμενο [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Μία παρουσία του [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) για τη σύλληψη συμβάντων OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions) με ορθογώνια περιοχή και αντικείμενο [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Μία παρουσία του [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) για τη σύλληψη συμβάντων OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Η ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Μία παρουσία του [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) για τη σύλληψη συμβάντων OCR. |
|
|  | useSpellCheker | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται ο ορθογραφικός ελεγκτής. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Λαμβάνει την ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Λαμβάνει τον διαχειριστή συμβάντων για τη σύλληψη γεγονότων OCR.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Λαμβάνει την τιμή που υποδεικνύει εάν χρησιμοποιείται ο ορθογραφικός ελεγκτής.


**Returns:**
boolean -  true  εάν χρησιμοποιείται ο ορθογραφικός ελεγκτής· διαφορετικά,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Λαμβάνει τις επιλογές προεπισκόπησης σελίδας που χρησιμοποιούνται για την απόδοση της σελίδας που παρέχεται στη μηχανή OCR.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Ορίζει τις επιλογές προεπισκόπησης σελίδας που χρησιμοποιούνται για την απόδοση της σελίδας που παρέχεται στη μηχανή OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Οι επιλογές προεπισκόπησης σελίδας. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Λαμβάνει τη γλώσσα που χρησιμοποιείται για την οπτική αναγνώριση χαρακτήρων.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Ορίζει τη γλώσσα που χρησιμοποιείται για την οπτική αναγνώριση χαρακτήρων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | Η τιμή enum του [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Ορίζει την ορθογώνια περιοχή που περιορίζει την περιοχή της σελίδας που χρησιμοποιείται για την αναγνώριση κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Το ορθογώνιο, ή  null  για σάρωση ολόκληρης της σελίδας. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Ορίζει τον διαχειριστή συμβάντων για τη σύλληψη συμβάντων OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Ο διαχειριστής συμβάντων. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Ορίζει την τιμή που υποδεικνύει εάν χρησιμοποιείται ο ορθογραφικός ελεγκτής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  για ενεργοποίηση ορθογραφικού ελέγχου. |
|

