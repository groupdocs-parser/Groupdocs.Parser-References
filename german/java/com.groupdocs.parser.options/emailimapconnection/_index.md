---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die E‑Mail‑Verbindungsinformationen für das IMAP‑Protokoll dar."
type: docs
weight: 14
url: /de/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Stellt die E‑Mail‑Verbindungsinformationen für das IMAP‑Protokoll dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getHost()](#getHost--) | Liefert den Hostnamen. |
|
|  | [getPort()](#getPort--) | Liefert die Portnummer. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Initialisiert eine neue Instanz der Klasse [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | host | java.lang.String | Der Hostname. |
|
|  | port | int | Die Portnummer. |
|
|  | userName | java.lang.String | Der Benutzername. |
|
|  | Passwort | java.lang.String | Das Passwort. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Liefert den Hostnamen.


**Returns:**
java.lang.String - Ein String-Wert, der den Hostnamen darstellt.

### getPort() {#getPort--}
```
public int getPort()
```


Liefert die Portnummer.


**Returns:**
int - Ein ganzzahliger Wert, der die Portnummer darstellt.

