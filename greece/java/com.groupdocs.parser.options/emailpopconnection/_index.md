---
title: "EmailPopConnection"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τις πληροφορίες σύνδεσης email για το πρωτόκολλο POP."
type: docs
weight: 15
url: /el/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

Αντιπροσωπεύει τις πληροφορίες σύνδεσης email για το πρωτόκολλο POP.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getHost()](#getHost--) | Λαμβάνει το όνομα κεντρικού υπολογιστή. |
|
|  | [getPort()](#getPort--) | Λαμβάνει τον αριθμό θύρας. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | host | java.lang.String | Το όνομα κεντρικού υπολογιστή. |
|
|  | port | int | Ο αριθμός θύρας. |
|
|  | userName | java.lang.String | Το όνομα χρήστη. |
|
|  | κωδικός | java.lang.String | Ο κωδικός. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Λαμβάνει το όνομα κεντρικού υπολογιστή.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το όνομα κεντρικού υπολογιστή.

### getPort() {#getPort--}
```
public int getPort()
```


Λαμβάνει τον αριθμό θύρας.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει τον αριθμό θύρας.

