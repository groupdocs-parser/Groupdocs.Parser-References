---
title: "EmailImapConnection"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta le informazioni di connessione email per il protocollo IMAP."
type: docs
weight: 14
url: /it/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Rappresenta le informazioni di connessione email per il protocollo IMAP.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getHost()](#getHost--) | Ottiene il nome host. |
|
|  | [getPort()](#getPort--) | Ottiene il numero di porta. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Inizializza una nuova istanza della classe [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | host | java.lang.String | Il nome host. |
|
|  | port | int | Il numero di porta. |
|
|  | userName | java.lang.String | Il nome utente. |
|
|  | password | java.lang.String | La password. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Ottiene il nome host.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome host.

### getPort() {#getPort--}
```
public int getPort()
```


Ottiene il numero di porta.


**Returns:**
int - Un valore intero che rappresenta il numero di porta.

