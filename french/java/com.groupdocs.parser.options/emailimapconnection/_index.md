---
title: "EmailImapConnection"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations de connexion email pour le protocole IMAP."
type: docs
weight: 14
url: /fr/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Représente les informations de connexion email pour le protocole IMAP.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getHost()](#getHost--) | Obtient le nom d'hôte. |
|
|  | [getPort()](#getPort--) | Obtient le numéro de port. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Initialise une nouvelle instance de la classe [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | host | java.lang.String | Le nom d'hôte. |
|
|  | port | int | Le numéro de port. |
|
|  | userName | java.lang.String | Le nom d'utilisateur. |
|
|  | password | java.lang.String | Le mot de passe. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Obtient le nom d'hôte.


**Returns:**
java.lang.String - Une valeur chaîne qui représente le nom d'hôte.

### getPort() {#getPort--}
```
public int getPort()
```


Obtient le numéro de port.


**Returns:**
int - Une valeur entière qui représente le numéro de port.

