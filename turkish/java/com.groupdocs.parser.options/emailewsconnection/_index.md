---
title: "EmailEwsConnection"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "EWS protokolü için e-posta bağlantı bilgisini temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

EWS protokolü için e-posta bağlantı bilgisini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | Yeni bir [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) sınıfının bir örneğini başlatır. |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Yeni bir [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | Posta kutusunun URI'sını alır. |
|
|  | [getDomain()](#getDomain--) | Alan adını alır. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


Yeni bir [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) sınıfının bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | Posta kutusunun URI'sı. |
|
|  | kullanıcıAdı | java.lang.String | Kullanıcı adı. |
|
|  | parola | java.lang.String | Parola. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


Yeni bir [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection) sınıfının bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | Posta kutusunun URI'sı. |
|
|  | domain | java.lang.String | Alan adı. |
|
|  | kullanıcıAdı | java.lang.String | Kullanıcı adı. |
|
|  | parola | java.lang.String | Parola. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


Posta kutusunun URI'sını alır.


**Returns:**
java.lang.String - Posta kutusunun URI'sını temsil eden bir dize değeri.

### getDomain() {#getDomain--}
```
public String getDomain()
```


Alan adını alır.


**Returns:**
java.lang.String - Alan adını temsil eden bir dize değeri.

