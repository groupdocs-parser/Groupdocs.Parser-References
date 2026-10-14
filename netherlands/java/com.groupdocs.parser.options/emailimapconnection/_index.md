---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Vertegenwoordigt de e-mailverbindinginformatie voor het IMAP-protocol."
type: docs
weight: 14
url: /nl/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

Vertegenwoordigt de e-mailverbindinginformatie voor het IMAP-protocol.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getHost()](#getHost--) | Haalt de hostnaam op. |
|
|  | [getPort()](#getPort--) | Haalt het poortnummer op. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Initialiseert een nieuw exemplaar van de klasse [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | host | java.lang.String | De hostnaam. |
|
|  | port | int | Het poortnummer. |
|
|  | userName | java.lang.String | De gebruikersnaam. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Haalt de hostnaam op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de hostnaam vertegenwoordigt.

### getPort() {#getPort--}
```
public int getPort()
```


Haalt het poortnummer op.


**Returns:**
int - Een gehele getalwaarde die het poortnummer vertegenwoordigt.

