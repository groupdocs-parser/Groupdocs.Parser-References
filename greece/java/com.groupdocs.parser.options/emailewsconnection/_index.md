---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τις πληροφορίες σύνδεσης email για το πρωτόκολλο EWS."
type: docs
weight: 13
url: /el/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Αντιπροσωπεύει τις πληροφορίες σύνδεσης email για το πρωτόκολλο EWS.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Λαμβάνει το URI του γραμματοκιβωτίου. |
|
|  | [getDomain()](#getDomain--) | Λαμβάνει το όνομα τομέα. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | Το URI του γραμματοκιβωτίου. |
|
|  | userName | java.lang.String | Το όνομα χρήστη. |
|
|  | κωδικός | java.lang.String | Ο κωδικός. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | Το URI του γραμματοκιβωτίου. |
|
|  | domain | java.lang.String | Το όνομα τομέα. |
|
|  | userName | java.lang.String | Το όνομα χρήστη. |
|
|  | κωδικός | java.lang.String | Ο κωδικός. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Λαμβάνει το URI του γραμματοκιβωτίου.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει ένα URI του γραμματοκιβωτίου.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Λαμβάνει το όνομα τομέα.


**Returns:**
java.lang.String - Μια τιμή συμβολοσειράς που αντιπροσωπεύει το όνομα τομέα.

