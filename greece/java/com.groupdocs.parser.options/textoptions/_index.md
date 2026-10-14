---
title: "TextOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή κειμένου."
type: docs
weight: 37
url: /el/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή κειμένου.

Μία παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) χρησιμοποιείται ως παράμετρος στη μέθοδο [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
και στις μεθόδους [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-). Δείτε τα παραδείγματα χρήσης εκεί.

Χρησιμοποιείται για να καθορίσει τη λειτουργία ακατέργαστης εξαγωγής κειμένου. Ένα κείμενο σε αυτή τη λειτουργία εξάγεται με μη ακριβή
αλλά είναι πιο γρήγορη από τη στάνταρ λειτουργία. Εάν η ακατέργαστη λειτουργία δεν υποστηρίζει τη μορφή του εγγράφου,
τότε αυτή η παράμετρος αγνοείται και χρησιμοποιείται η στάνταρ λειτουργία.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με την επιλογή χρήσης OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με τη δυνατότητα ορισμού επιλογών OCR. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Αποκτά την τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία. |
|
|  | [isUseOcr()](#isUseOcr--) | Αποκτά την τιμή που υποδεικνύει εάν χρησιμοποιείται το OCR Connector για την εξαγωγή κειμένου. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Αποκτά τις πρόσθετες επιλογές για τη λειτουργικότητα OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Αποκτά την τιμή που υποδεικνύει εάν οι σημειώσεις περιλαμβάνονται στο εξαγόμενο κείμενο. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Ορίζει την τιμή που υποδεικνύει εάν οι σημειώσεις περιλαμβάνονται στο εξαγόμενο κείμενο. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με την επιλογή χρήσης OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία. |
|
|  | useOcr | boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή κειμένου. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TextOptions](../../com.groupdocs.parser.options/textoptions) με τη δυνατότητα ορισμού επιλογών OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Η τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία. |
|
|  | useOcr | boolean | Η τιμή που υποδεικνύει εάν η λειτουργία OCR χρησιμοποιείται για την εξαγωγή κειμένου. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Οι πρόσθετες επιλογές για τη λειτουργικότητα OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Αποκτά την τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία.


**Returns:**
boolean -  true  εάν χρησιμοποιείται η ακατέργαστη λειτουργία· διαφορετικά,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Αποκτά την τιμή που υποδεικνύει εάν οι σημειώσεις περιλαμβάνονται στο εξαγόμενο κείμενο. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean -  true  εάν οι σημειώσεις περιλαμβάνονται· διαφορετικά,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Ορίζει την τιμή που υποδεικνύει εάν οι σημειώσεις περιλαμβάνονται στο εξαγόμενο κείμενο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  για να συμπεριληφθούν οι σημειώσεις στο εξαγόμενο κείμενο. |
|

