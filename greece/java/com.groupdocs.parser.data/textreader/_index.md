---
title: "TextReader"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει έναν αναγνώστη που μπορεί να διαβάσει μια διαδοχική σειρά χαρακτήρων."
type: docs
weight: 29
url: /el/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Αντιπροσωπεύει έναν αναγνώστη που μπορεί να διαβάσει μια διαδοχική σειρά χαρακτήρων.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Διαβάζει μια γραμμή χαρακτήρων από τον αναγνώστη κειμένου και επιστρέφει τα δεδομένα ως συμβολοσειρά. |
|
|  | [readToEnd()](#readToEnd--) | Διαβάζει όλους τους χαρακτήρες από την τρέχουσα θέση μέχρι το τέλος του αναγνώστη κειμένου και τους επιστρέφει ως μία συμβολοσειρά. |
|
|  | [dispose()](#dispose--) | Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το αντικείμενο [TextReader](../../com.groupdocs.parser.data/textreader). |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


Διαβάζει μια γραμμή χαρακτήρων από τον αναγνώστη κειμένου και επιστρέφει τα δεδομένα ως συμβολοσειρά.


**Returns:**
java.lang.String - Η επόμενη γραμμή από τον αναγνώστη, ή  null  εάν έχουν διαβαστεί όλοι οι χαρακτήρες.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Διαβάζει όλους τους χαρακτήρες από την τρέχουσα θέση μέχρι το τέλος του αναγνώστη κειμένου και τους επιστρέφει ως μία συμβολοσειρά.


**Returns:**
java.lang.String - Μια συμβολοσειρά που περιέχει όλους τους χαρακτήρες από την τρέχουσα θέση μέχρι το τέλος του αναγνώστη κειμένου.

### dispose() {#dispose--}
```
public void dispose()
```


Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το αντικείμενο [TextReader](../../com.groupdocs.parser.data/textreader).


