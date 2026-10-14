---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar e-postanslutningsinformationen för IMAP-protokollet."
type: docs
weight: 14
url: /sv/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Representerar e-postanslutningsinformationen för IMAP-protokollet.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getHost()](#getHost--) | Hämtar värdnamnet. |
|
|  | [getPort()](#getPort--) | Hämtar portnumret. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Initierar en ny instans av klassen [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | host | java.lang.String | Värdnamnet. |
|
|  | port | int | Portnumret. |
|
|  | userName | java.lang.String | Användarnamnet. |
|
|  | lösenord | java.lang.String | Lösenordet. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Hämtar värdnamnet.


**Returns:**
java.lang.String - Ett strängvärde som representerar värdnamnet.

### getPort() {#getPort--}
```
public int getPort()
```


Hämtar portnumret.


**Returns:**
int - Ett heltalsvärde som representerar portnumret.

