---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή μορφοποιημένου κειμένου."
type: docs
weight: 21
url: /el/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Παρέχει τις επιλογές που χρησιμοποιούνται για την εξαγωγή μορφοποιημένου κειμένου.

Μια παρουσία της κλάσης [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) χρησιμοποιείται ως παράμετρος στη μέθοδο [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
και τις μεθόδους [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-). Δείτε τα παραδείγματα χρήσης εκεί.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) χωρίς ορισμένη λειτουργία. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getMode()](#getMode--) | Λαμβάνει τη λειτουργία εξαγωγής μορφοποιημένου κειμένου. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Ορίζει τη λειτουργία εξαγωγής μορφοποιημένου κειμένου. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) χωρίς ορισμένη λειτουργία.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Η λειτουργία εξαγωγής μορφοποιημένου κειμένου. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Λαμβάνει τη λειτουργία εξαγωγής μορφοποιημένου κειμένου.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Ορίζει τη λειτουργία εξαγωγής μορφοποιημένου κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Η απαρίθμηση [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) που περιέχει μια λειτουργία εξαγωγής μορφοποιημένου κειμένου. |
|

