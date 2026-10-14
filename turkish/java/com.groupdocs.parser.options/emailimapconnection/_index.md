---
title: "EmailImapConnection"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "IMAP protokolü için e-posta bağlantı bilgisini temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

IMAP protokolü için e-posta bağlantı bilgisini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Yeni bir [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getHost()](#getHost--) | Ana bilgisayar adını alır. |
|
|  | [getPort()](#getPort--) | Bağlantı noktasının numarasını alır. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


Yeni bir [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ana bilgisayar | java.lang.String | Ana bilgisayar adı. |
|
|  | bağlantı noktası | int | Bağlantı noktası numarası. |
|
|  | kullanıcıAdı | java.lang.String | Kullanıcı adı. |
|
|  | parola | java.lang.String | Parola. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Ana bilgisayar adını alır.


**Returns:**
java.lang.String - Ana bilgisayar adını temsil eden bir dize değeri.

### getPort() {#getPort--}
```
public int getPort()
```


Bağlantı noktasının numarasını alır.


**Returns:**
int - Bağlantı noktasını temsil eden bir tam sayı değeri.

