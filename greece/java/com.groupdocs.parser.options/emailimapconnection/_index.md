---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τις πληροφορίες σύνδεσης email για το πρωτόκολλο IMAP."
type: docs
weight: 14
url: /el/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Αντιπροσωπεύει τις πληροφορίες σύνδεσης email για το πρωτόκολλο IMAP.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getHost()](#getHost--) | Λαμβάνει το όνομα κεντρικού υπολογιστή. |
|
|  | [getPort()](#getPort--) | Λαμβάνει τον αριθμό θύρας. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


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

