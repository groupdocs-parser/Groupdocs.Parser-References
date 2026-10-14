---
title: "EmailPopConnection"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les informations de connexion email pour le protocole POP."
type: docs
weight: 15
url: /fr/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

Représente les informations de connexion email pour le protocole POP.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getHost()](#getHost--) | Obtient le nom d'hôte. |
|
|  | [getPort()](#getPort--) | Obtient le numéro de port. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


Initialise une nouvelle instance de la classe [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection).


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

