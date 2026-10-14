---
title: "EmailEwsConnection"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni di connessione email per il protocollo EWS."
type: docs
weight: 13
url: /it/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Rappresenta le informazioni di connessione email per il protocollo EWS.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Ottiene l'URI della casella di posta. |
|
|  | [getDomain()](#getDomain--) | Ottiene il nome del dominio. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Inizializza una nuova istanza della classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | L'URI della casella di posta. |
|
|  | userName | java.lang.String | Il nome utente. |
|
|  | password | java.lang.String | La password. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Inizializza una nuova istanza della classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | L'URI della casella di posta. |
|
|  | domain | java.lang.String | Il nome del dominio. |
|
|  | userName | java.lang.String | Il nome utente. |
|
|  | password | java.lang.String | La password. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Ottiene l'URI della casella di posta.


**Returns:**
java.lang.String - Un valore stringa che rappresenta un URI della casella di posta.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Ottiene il nome del dominio.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome del dominio.

