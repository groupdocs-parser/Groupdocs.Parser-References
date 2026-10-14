---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar e-postanslutningsinformationen för EWS-protokollet."
type: docs
weight: 13
url: /sv/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

Representerar e-postanslutningsinformationen för EWS-protokollet.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Initierar en ny instans av klassen [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Hämtar URI:n för brevlådan. |
|
|  | [getDomain()](#getDomain--) | Hämtar domännamnet. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Initierar en ny instans av klassen [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI:n för brevlådan. |
|
|  | userName | java.lang.String | Användarnamnet. |
|
|  | lösenord | java.lang.String | Lösenordet. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Initierar en ny instans av klassen [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI:n för brevlådan. |
|
|  | domain | java.lang.String | Domännamnet. |
|
|  | userName | java.lang.String | Användarnamnet. |
|
|  | lösenord | java.lang.String | Lösenordet. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Hämtar URI:n för brevlådan.


**Returns:**
java.lang.String - Ett strängvärde som representerar en URI för brevlådan.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Hämtar domännamnet.


**Returns:**
java.lang.String - Ett strängvärde som representerar domännamnet.

