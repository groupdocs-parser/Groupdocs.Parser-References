---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die E‑Mail‑Verbindungsinformationen für das EWS‑Protokoll dar."
type: docs
weight: 13
url: /de/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Stellt die E‑Mail‑Verbindungsinformationen für das EWS‑Protokoll dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Ermittelt die URI des Postfachs. |
|
|  | [getDomain()](#getDomain--) | Ermittelt den Domainnamen. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Initialisiert eine neue Instanz der Klasse [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | Die URI des Postfachs. |
|
|  | userName | java.lang.String | Der Benutzername. |
|
|  | Passwort | java.lang.String | Das Passwort. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Initialisiert eine neue Instanz der Klasse [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | Die URI des Postfachs. |
|
|  | domain | java.lang.String | Der Domainname. |
|
|  | userName | java.lang.String | Der Benutzername. |
|
|  | Passwort | java.lang.String | Das Passwort. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Ermittelt die URI des Postfachs.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der die URI des Postfachs darstellt.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Ermittelt den Domainnamen.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Domainnamen darstellt.

