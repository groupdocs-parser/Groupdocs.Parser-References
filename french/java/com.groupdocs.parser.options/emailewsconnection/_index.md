---
title: "EmailEwsConnection"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations de connexion email pour le protocole EWS."
type: docs
weight: 13
url: /fr/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Représente les informations de connexion email pour le protocole EWS.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Obtient l'URI de la boîte aux lettres. |
|
|  | [getDomain()](#getDomain--) | Obtient le nom de domaine. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Initialise une nouvelle instance de la classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | L'URI de la boîte aux lettres. |
|
|  | userName | java.lang.String | Le nom d'utilisateur. |
|
|  | password | java.lang.String | Le mot de passe. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Initialise une nouvelle instance de la classe [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | L'URI de la boîte aux lettres. |
|
|  | domain | java.lang.String | Le nom de domaine. |
|
|  | userName | java.lang.String | Le nom d'utilisateur. |
|
|  | password | java.lang.String | Le mot de passe. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Obtient l'URI de la boîte aux lettres.


**Returns:**
java.lang.String - Une valeur chaîne qui représente l'URI de la boîte aux lettres.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Obtient le nom de domaine.


**Returns:**
java.lang.String - Une valeur chaîne qui représente le nom de domaine.

