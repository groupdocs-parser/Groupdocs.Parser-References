---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τα δεδομένα για τη μέθοδο."
type: docs
weight: 17
url: /el/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Παρέχει τα δεδομένα για τη μέθοδο [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) με ορθογώνια περιοχή. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getUri()](#getUri--) | Αποκτά το URI του εξωτερικού πόρου. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Αποκτά το URI του εξωτερικού πόρου. |
|
|  | [isSkipped()](#isSkipped--) | Αποκτά την τιμή που υποδεικνύει εάν η φόρτωση του εξωτερικού πόρου πρέπει να παραλειφθεί. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Ορίζει την τιμή που υποδεικνύει εάν η φόρτωση του εξωτερικού πόρου πρέπει να παραλειφθεί. |
|
|  | [getData()](#getData--) | Αποκτά τα δεδομένα χρήστη. |
|
|  | [setData(byte[] data)](#setData-byte---) | Ορίζει τα δεδομένα χρήστη. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) με ορθογώνια περιοχή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | uri | java.lang.String | URI του εξωτερικού πόρου. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Αποκτά το URI του εξωτερικού πόρου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το URI του εξωτερικού πόρου.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Αποκτά το URI του εξωτερικού πόρου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | uri | java.lang.String | Μια τιμή συμβολοσειράς που αντιπροσωπεύει ένα νέο URI του εξωτερικού πόρου. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Αποκτά την τιμή που υποδεικνύει εάν η φόρτωση του εξωτερικού πόρου πρέπει να παραλειφθεί.


**Returns:**
boolean - true εάν η φόρτωση του εξωτερικού πόρου πρέπει να παραλειφθεί· διαφορετικά, false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Ορίζει την τιμή που υποδεικνύει εάν η φόρτωση του εξωτερικού πόρου πρέπει να παραλειφθεί.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | παραλειφθεί | boolean | true εάν η φόρτωση του εξωτερικού πόρου πρέπει να παραλειφθεί· διαφορετικά, false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Αποκτά τα δεδομένα χρήστη.


**Returns:**
byte[] - Ο πίνακας byte με το περιεχόμενο χρήστη του εξωτερικού πόρου. null εάν δεν έχει οριστεί.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Ορίζει τα δεδομένα χρήστη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | byte[] | Ο πίνακας byte με το περιεχόμενο χρήστη του εξωτερικού πόρου. null εάν δεν έχει οριστεί. |
|

