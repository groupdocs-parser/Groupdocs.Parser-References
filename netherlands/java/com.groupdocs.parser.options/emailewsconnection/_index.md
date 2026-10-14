---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Vertegenwoordigt de e-mailverbindinginformatie voor het EWS-protocol."
type: docs
weight: 13
url: /nl/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Vertegenwoordigt de e-mailverbindinginformatie voor het EWS-protocol.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) klasse. |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Haalt de URI van de mailbox op. |
|
|  | [getDomain()](#getDomain--) | Haalt de domeinnaam op. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Initialiseert een nieuw exemplaar van de [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | De URI van de mailbox. |
|
|  | userName | java.lang.String | De gebruikersnaam. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Initialiseert een nieuw exemplaar van de [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | De URI van de mailbox. |
|
|  | domain | java.lang.String | De domeinnaam. |
|
|  | userName | java.lang.String | De gebruikersnaam. |
|
|  | wachtwoord | java.lang.String | Het wachtwoord. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Haalt de URI van de mailbox op.


**Returns:**
java.lang.String - Een tekenreekswaarde die een URI van de mailbox weergeeft.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Haalt de domeinnaam op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de domeinnaam weergeeft.

